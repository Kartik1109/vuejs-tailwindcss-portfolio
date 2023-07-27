<script>
export default {
	setup() {
		return {
			bios: [
			{
					id: 1,
					bio:'Goooood Day!'
			},
				{
					id: 2,
					bio:
						' My name is Kartik Chaudhari. I just finished my third year at McMaster University in the field of Software Engineering. I am currently on my internship period and have gained some valuable skills over the years through academic courses and internships experiences. I like learning something new everyday. But what I love is implementing them! Haha :) Just like this website! On Weekends I usually participate in Hackathons and in my free time I like doing leetcode problems! (apart from Netflix obviously) '
				},
				{
					id: 3,
					bio:
						'Apart from a bunch of technical experience, I also have strong leadership skills and a good ability to communicate ideas. I have been the Head Boy of my school and have also been a Vice President for a Software Club at McMaster University. I have also been a Teaching Assistant and a Research Assistant in the field of software which have deepened my understanding of not only technical but soft skills as well. '
				},

			],
		};
	},
};
</script>

<template>
	<div class="block sm:flex sm:gap-10 mt-10 sm:mt-20">
		<!-- About profile image -->
		<div class="w-full sm:w-1/4 mb-7 sm:mb-0">
			<img
				src="@/assets/images/profile.jpg"
				class="rounded-xl w-96"
				alt=""
			/>
		</div>

		<!-- About details -->
		<div class="w-full sm:w-3/4 text-left">
			<p
				v-for="bio in bios"
				:key="bio.id"
				class="font-general-regular mb-4 text-ternary-dark dark:text-ternary-light text-lg"
			>
				{{ bio.bio }}
			</p>
		</div>
	</div>
</template>
