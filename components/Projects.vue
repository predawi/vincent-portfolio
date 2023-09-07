<template>
	<section class="projects">
		<div class="container">
			<h2 class="typo-t2 projects__title">Latest works</h2>

			<p class="typo-p">I’ve been creating digital products and experiences for more than 7 years in freelance. I had the chance to work for a lot of different industries and companies</p>
		</div>

		<div class="projects__list">

			<!-- One tile projet -->
			<div class="container">
				<div class="projects__item">
					<NuxtLink to="/projects/anoti" class="projects__link">
						<div class="projects__infos">
							<h3 class="projects__title">BNP Paribas</h3>
							<span class="typo-category projects__category">SAAS COMPLIANCE</span>
						</div>
					</NuxtLink>
				</div>
			</div>
			<!-- // -->
			
			<!-- Three tiles projects -->
			<div class="projects__row">
				<div class="projects__item">
					<NuxtLink to="/projects/anoti" class="projects__link">
						<div class="projects__infos">
							<h3 class="projects__title">BNP Paribas</h3>
							<span class="typo-category projects__category">SAAS COMPLIANCE</span>
						</div>
					</NuxtLink>
				</div>

				<div class="projects__item">
					<NuxtLink to="/projects/anoti" class="projects__link">
						<div class="projects__infos">
							<h3 class="projects__title">BNP Paribas</h3>
							<span class="typo-category projects__category">SAAS COMPLIANCE</span>
						</div>
					</NuxtLink>
				</div>

				<div class="projects__item">
					<NuxtLink to="/projects/anoti" class="projects__link">
						<div class="projects__infos">
							<h3 class="projects__title">BNP Paribas</h3>
							<span class="typo-category projects__category">SAAS COMPLIANCE</span>
						</div>
					</NuxtLink>
				</div>
			</div>
			<!-- // -->

			<!-- One tile projet -->
			<div class="container">
				<div class="projects__item">
					<NuxtLink to="/projects/anoti" class="projects__link">
						<div class="projects__infos">
							<h3 class="projects__title">BNP Paribas</h3>
							<span class="typo-category projects__category">SAAS COMPLIANCE</span>
						</div>
					</NuxtLink>
				</div>
			</div>
			<!-- // -->

		</div>
	</section>
</template>

<script>
export default {
	name: 'NuxtProjects'
}
</script>
