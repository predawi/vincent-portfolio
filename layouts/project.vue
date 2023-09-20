<template>
	<div>
		<HeaderBanner />
		<nuxt />
		<Footer />
		
	</div>
</template>

<script>
import HeaderBanner from '~/components/HeaderBanner.vue';
import Footer from '~/components/Footer.vue';

export default {
	components: {
		HeaderBanner,
		Footer,
	},
	head: {
		bodyAttrs: {
			class: 'project-template'
		}
	},
};
</script>

<style lang="scss">
.project-template {
	background: $maingrey;

	.container {
		@include tablet {
			max-width: 1060px;
		}
	}
}
</style>
