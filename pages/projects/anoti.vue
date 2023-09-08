<template>
	<div>
		<project-intro title="Anoti" skills="UX & UI"
			intro="I collaborated with Anoti, a startup tackling corporate compliance issues, to form their visual identity, and construct their primary website with the intent to attract customers. The Saas platform is the tool they offer to businesses" />

		<project-img 
			imgSrc="/projects/anoti/anoti-01.png" 
			imgAlt="Anoti image 01" 
			mobileWidth="100%" 
			desktopWidth="70%" 
			marginTop="70px" 
			alignment="right" 
			noPadding="true"
			caption="Workshop : “User needs // Served by”" />

	</div>
</template>
<script>
import ProjectIntro from '~/components/ProjectIntro.vue';
import ProjectImg from '~/components/ProjectImg.vue';

export default {
	layout: 'project',
	name: 'Anoti',
	components: {
		ProjectIntro,
		ProjectImg,
	},
}
</script>
  