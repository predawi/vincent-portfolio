<template>
	<header class="header" id="header">
		<div class="header__inner">
			<Logo />
			<BaseNav />
		</div>
	</header>
</template>

<script>
import Logo from '~/components/Logo.vue';
import BaseNav from '~/components/BaseNav.vue';

export default {
	components: {
		Logo,
		BaseNav,
	}
};
</script>
  