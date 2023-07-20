<template>
  <div>
    <HeaderBanner/>
    <Intro/>
    <Projects/>
  </div>
</template>

<script>
import HeaderBanner from '~/components/HeaderBanner.vue';
import Intro from '~/components/Intro.vue';
import Projects from '~/components/Projects.vue';

export default {
  name: 'IndexPage'
}
</script>
