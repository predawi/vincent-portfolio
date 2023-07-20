<!-- Please remove this file from your project -->
<template>
	<section class="projects">
		<div class="container">
			<h2 class="typo-t2 projects__title">Latest works</h2>

			<p class="base-p">I’ve been creating digital products and experiences for more than 7 years in freelance. I had the chance to work for a lot of different industries and companies</p>
		</div>

		<div class="projects__list">
			<div class="container">
				<div class="projects__item">
					<NuxtLink to="/projects/anoti" class="base-link intro__link">ANOTI</NuxtLink>
				</div>
			</div>

			<div class="projects__row">
				<div class="projects__item">
					<NuxtLink to="/projects/anoti" class="base-link intro__link">ANOTI</NuxtLink>
				</div>
				<div class="projects__item">
					<NuxtLink to="/projects/anoti" class="base-link intro__link">ANOTI</NuxtLink>
				</div>
				<div class="projects__item">
					<NuxtLink to="/projects/anoti" class="base-link intro__link">ANOTI</NuxtLink>
				</div>
			</div>
		</div>
	</section>
</template>

<script>
export default {
	name: 'NuxtProjects'
}
</script>
