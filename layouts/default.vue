<template>
    <div>
        <HeaderBanner/>
        <nuxt />
        <Footer/>
    </div>
</template>

<script>
import HeaderBanner from '~/components/HeaderBanner.vue';
import Footer from '~/components/Footer.vue';

export default {
  components: {
    HeaderBanner,
    Footer,
  }
};
</script>
