<template>
  <div>
    <HeaderBanner/>
    <Intro/>
    <Projects/>
    <Clients/>
    <Reviews/>
  </div>
</template>

<script>
import HeaderBanner from '~/components/HeaderBanner.vue';
import Intro from '~/components/Intro.vue';
import Projects from '~/components/Projects.vue';
import Clients from '~/components/Clients.vue';
import Reviews from '~/components/Reviews.vue';

export default {
  name: 'IndexPage'
}
</script>
