<script>
export default {
	setup() {
		return {
			bios: [
				{
					id: 1,
					bio:
						'As a seasoned Front-end Engineer, I bring a wealth of expertise in crafting contemporary web applications, websites, design systems, and widgets, with a background that spans from innovative startups to established enterprise environments.',
				},
				{
					id: 2,
					bio:
						'My proficiency encompasses UI/UX design, software development, testing, and debugging, with a particular focus on Typescript, JavaScript, Vue 3 (including migration projects from Vue 2), Quasar Framework, and Nuxt.js. I am an enthusiastic explorer of Typescript and an advocate for Functional programming principles.',
				},
				{
					id: 3,
					bio:
						'Recognized as a highly skilled specialist in Vue and CSS, I excel in problem-solving, enhancing user experience, and optimizing performance with a strong emphasis on user-centric design and usability.',
				},
			],
		};
	},
};
</script>

<template>
	<div class="block sm:flex sm:gap-10 mt-10 sm:mt-20">
		<!-- About details -->
		<div class="w-full sm:w-4/4 text-left">
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
