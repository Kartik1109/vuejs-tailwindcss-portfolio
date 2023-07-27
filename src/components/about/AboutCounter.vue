<script>
export default {
	data: () => {
		return {
			projectsTitle: 'McMaster International Student Award',
			experienceTitle: 'Hackathon Wins!',
			githubTitle: 'Cumulative GPA',
			feedbackTitle: 'Best Engineering Project Award',
			projectTitle2: ' Anticipated Graduation Year'
		};
	},
};
</script>

<template>
	<div class="mt-10 sm:mt-20 bg-primary-light dark:bg-ternary-dark shadow-sm">
		<!-- About me counters -->
		<div
			class="font-general-regular container mx-auto py-20 block sm:flex sm:justify-between sm:items-center"
		>
		<!-- Projects completed counter -->
		<div class="mb-20 sm:mb-0">
				<div class="font-general-medium text-4xl font-bold text-secondary-dark dark:text-secondary-light mb-2" aria-label="About Status Counter">
  2020
</div>
				<span
					class="block text-md text-ternary-dark dark:text-ternary-light"
				>
					{{ projectsTitle }}
				</span>
			</div>
			<!-- Years of experience counter -->
			<div class="mb-20 sm:mb-0">
				<div class="font-general-medium text-4xl font-bold text-secondary-dark dark:text-secondary-light mb-2" aria-label="About Status Counter">
  4/5
</div>
				<span
					class="block text-md text-ternary-dark dark:text-ternary-light"
				>
					{{ experienceTitle }}
				</span>
			</div>
			<!-- Positive feedback counter -->
			<div class="mb-20 sm:mb-0">
				<div class="font-general-medium text-4xl font-bold text-secondary-dark dark:text-secondary-light mb-2" aria-label="About Status Counter">
  2021
</div>
				<span
					class="block text-md text-ternary-dark dark:text-ternary-light"
				>
					{{ feedbackTitle }}
				</span>
			</div>


			<!-- GitHub stars counter -->
			<div class="mb-20 sm:mb-0">
				<div class="font-general-medium text-4xl font-bold text-secondary-dark dark:text-secondary-light mb-2" aria-label="About Status Counter">
  3.9/4.0
</div>
				<span
					class="block text-md text-ternary-dark dark:text-ternary-light"
					>{{ githubTitle }}</span
				>
			</div>

			
			
			<div class="mb-20 sm:mb-0">
				<div class="font-general-medium text-4xl font-bold text-secondary-dark dark:text-secondary-light mb-2" aria-label="About Status Counter">
  2025
</div>
				<span
					class="block text-md text-ternary-dark dark:text-ternary-light"
				>
					{{ projectTitle2 }}
				</span>
			</div>
		</div>
	</div>
</template>
