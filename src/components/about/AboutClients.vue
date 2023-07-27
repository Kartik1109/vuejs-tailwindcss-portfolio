<script>
import AboutClientSingle from './AboutClientSingle.vue';

export default {
	components: {
		AboutClientSingle,
	},
	data: () => {
		return {
			clientsHeading: 'Some of my Key Skills',
			clients: [
				{
					id: 1,
					title: 'Amazon',
					img: require('@/assets/images/brands/1.png'),
				},
				{
					id: 2,
					title: 'Sony',
					img: require('@/assets/images/brands/2.png'),
				},
				{
					id: 3,
					title: 'Adidas',
					img: require('@/assets/images/brands/3.png'),
				},
				{
					id: 4,
					title: 'FILA',
					img: require('@/assets/images/brands/4.png'),
				},
				{
					id: 5,
					title: 'NB',
					img: require('@/assets/images/brands/5.png'),
				},
				{
					id: 6,
					title: 'SAMSUNG',
					img: require('@/assets/images/brands/6.png'),
				},
				{
					id: 7,
					title: 'CANON',
					img: require('@/assets/images/brands/7.png'),
				},
				{
					id: 8,
					title: 'PUMA',
					img: require('@/assets/images/brands/8.png'),
				},
				{
					id: 9,
					title: 'PUMA',
					img: require('@/assets/images/brands/9.png'),
				},
				{
					id: 10,
					title: 'PUMA',
					img: require('@/assets/images/brands/10.png'),
				},
				{
					id: 11,
					title: 'PUMA',
					img: require('@/assets/images/brands/11.jpg'),
				},
				{
					id: 12,
					title: 'PUMA',
					img: require('@/assets/images/brands/12.jpg'),
				},
				{
					id: 8,
					title: 'PUMA',
					img: require('@/assets/images/brands/13.webp'),
				},
				{
					id: 8,
					title: 'PUMA',
					img: require('@/assets/images/brands/14.png'),
				},
				{
					id: 8,
					title: 'PUMA',
					img: require('@/assets/images/brands/15.png'),
				},
			],
		};
	},
};
</script>

<template>
	<div class="mt-10 sm:mt-20">
		<p
			class="font-general-medium text-2xl sm:text-3xl text-primary-dark dark:text-primary-light"
		>
			{{ clientsHeading }}
		</p>
		<div class="grid grid-cols-2 sm:grid-cols-4 mt-10 sm:mt-14 gap-2">
			<AboutClientSingle
				v-for="client in clients"
				:key="client.id"
				:client="client"
			/>
		</div>
	</div>
</template>
