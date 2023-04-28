<script>
import img2 from '../assets/img/h3-rev-img-2.png'
import img4 from '../assets/img/h3-rev-img-4.png'
import img6 from '../assets/img/h3-rev-img-6.png'
import bkg1 from '../assets/img/h3-rev-img-1.png'
import bkg3 from '../assets/img/h3-rev-img-3.png'
import bkg5 from '../assets/img/h3-rev-img-5.png'
import CarouselHeader from './CarouselHeader.vue';
import NavbarHeader from './NavbarHeader.vue';
export default {
  name: 'AppHeader',
  components: {
    NavbarHeader,
    CarouselHeader,
    img2,
    img4,
    img6,
    bkg1,
    bkg3,
    bkg5
  },
  data() {
    return {
      pages: [
        {
          title: 'HOME',
          url: '#sectionHome'
        },
        {
          title: 'PAGES',
          url: '#'
        },
        {
          title: 'MENU',
          url: '#',
        }
      ],

      links: [
        {
          title: 'EVENT',
          url: '#calendar'
        },
        {
          title: 'BLOG',
          url: '#blog'
        },
        {
          title: 'LANDING',
          url: '#landing'
        }
      ],

      images: [
        img2,
        img4,
        img6,
      ],
      background: [
        bkg1,
        bkg3,
        bkg5,
      ],
    };
  },
}
</script>
<template>
  <header>
    <NavbarHeader :pages="pages" :links="links" />
    <CarouselHeader :images="images" :background="background" />
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