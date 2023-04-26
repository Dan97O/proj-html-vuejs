<script>


import CarouselHeader from './CarouselHeader.vue';
import NavbarHeader from './NavbarHeader.vue';
export default {
  name: 'AppHeader',
  components: {
    NavbarHeader,
    CarouselHeader,
  },
}
</script>
<template>
  <header>
    <NavbarHeader />
    <CarouselHeader />
  </header>
</template>


<style lang="scss" scoped>
@import "../assets/scss/partials/variables";

header {
  background-color: black;
}
</style>