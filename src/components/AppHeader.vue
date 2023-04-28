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
  background-color: $background_dark;
  font-family: "Poppins";
  font-size: 16px;
  background-image: url('../assets/img/costellazione.jpeg');
  background-repeat: round;
}
</style>