<template>
	<div>
		<HeaderBanner />
		<nuxt />

		<client-only>
			<div class="d-flex">
				<project-nav :link="this.getPrevPage.slug" :title="this.getPrevPage.name" :category="this.getPrevPage.category" />
				<project-nav :link="this.getNextPage.slug" :title="this.getNextPage.name" :category="this.getNextPage.category" />
			</div>
		</client-only>
		<Footer />
	</div>
</template>

<script>
import projects from '../data/project-list.json';

import HeaderBanner from '~/components/HeaderBanner.vue';
import Footer from '~/components/Footer.vue';
import ProjectNav from '~/components/ProjectNav.vue';

export default {
	components: {
		HeaderBanner,
		ProjectNav,
		Footer,
	},
	head: {
		bodyAttrs: {
			class: 'project-template'
		}
	},
	computed: {
		getPrevPage() {
			let currentSlug = this.$route.path.substring(this.$route.path.lastIndexOf('/') + 1);
			let index = -1;
			let val = currentSlug;
			let filteredObj = projects.find(function(item, i) {
				if (item.slug === val) {
					index = i;
					return i;
				}
			});

			return projects[index - 1] ? projects[index - 1] : projects[projects.length - 1];
		},
		getNextPage() {
			let currentSlug = this.$route.path.substring(this.$route.path.lastIndexOf('/') + 1);
			let index = -1;
			let val = currentSlug;
			let filteredObj = projects.find(function(item, i) {
				if (item.slug === val){
					index = i;
					return i;
				}
			});

			return projects[index + 1] ? projects[index + 1] : projects[0];
		}
	},
};
</script>

<style lang="scss">
.project-template {
	background: $maingrey;
}

.container {
	@include tablet {
		max-width: 1060px;
	}
}
</style>
