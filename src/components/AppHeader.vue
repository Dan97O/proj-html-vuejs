<script>
import img2 from '../assets/img/h3-rev-img-2.png'
import img4 from '../assets/img/h3-rev-img-4.png'
import img6 from '../assets/img/h3-rev-img-6.png'
import bkg1 from '../assets/img/h3-rev-img-1.png'
import bkg3 from '../assets/img/h3-rev-img-3.png'
import bkg5 from '../assets/img/h3-rev-img-5.png'


import NavbarHeader from './NavbarHeader.vue';
export default {
  name: 'AppHeader',
  components: {
    NavbarHeader,
    img2,
    img4,
    img6,
    bkg1,
    bkg3,
    bkg5
  },

  data() {
    return {
      images: [
        img2,
        img4,
        img6,
      ],
       : [
        bkg1,
        bkg3,
        bkg5,
      ],
      currentImage: 0,
    };
  },
  methods: {
    prevImage() {
      if (this.currentImage === 0) {
        this.currentImage = this.images.length - 1;
        console.log('premuto prev');
      } else {
        this.currentImage--;
      }
    },
    nextImage() {
      if (this.currentImage === this.images.length - 1) {
        this.currentImage = 0;
        console.log('premuto next');
      } else {
        this.currentImage++;
      }
    },
  },

}
</script>
<template>
  <header>
    <NavbarHeader />
    <section class="d-flex justify-content-center">
      <div class="advance d-flex justify-content-between">
        <div class="prev d-flex align-items-center">
          <button @click="prevImage()">PREV</button>
        </div>
        <div class="carousel d-flex justify-content-center"
          :style="{ 'background-image': `url(${background[currentImage]})` }">
          <img v-for="image in images" :src="image" :class="{ active: image === images[currentImage] }" alt="">

        </div>
        <div class="next d-flex align-items-center">
          <button @click="nextImage()">NEXT</button>
        </div>
      </div>
    </section>
  </header>
</template>


<style lang="scss" scoped>
@import "../assets/scss/partials/variables";

header {
  height: 600px;
  background-color: black;

  .advance {
    width: 100%;

    .prev button,
    .next button {
      padding: 10px;
      background-color: $header_text_color;
      color: $header_btn;
      border: none;
      border-radius: 50% 50% 0 0;
      writing-mode: vertical-rl;
      height: 40px;
      margin-left: -8px;
      margin-right: -8px;
    }

    .prev button {
      transform: rotate(90deg);
    }

    .next button {
      transform: rotate(-90deg);
    }

    .carousel {
      text-align: center;
      background-repeat: no-repeat;
      width: 53%;
      object-fit: contain;

      img {
        height: 400px;
      }

      img:not(.active) {
        display: none;
      }

      img.active {
        display: block;
      }
    }
  }
}
</style>