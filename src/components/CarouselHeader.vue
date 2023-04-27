<script>
import img2 from '../assets/img/h3-rev-img-2.png'
import img4 from '../assets/img/h3-rev-img-4.png'
import img6 from '../assets/img/h3-rev-img-6.png'
import bkg1 from '../assets/img/h3-rev-img-1.png'
import bkg3 from '../assets/img/h3-rev-img-3.png'
import bkg5 from '../assets/img/h3-rev-img-5.png'
export default {
  name: 'CarouselHeader',
  components: {
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
      background: [
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
  <div class="container-fluid p-0">
    <div class="row" :style="{ 'background-image': `url(${background[currentImage]})` }">
      <div class="col-12">
        <div class="d-flex justify-content-center">
          <div class="advance d-flex justify-content-between">
            <div class="prev d-flex align-items-center">
              <button @click="prevImage()">PREV</button>
            </div>
            <!-- /prev -->
            <div class="carousel d-flex justify-content-center pb-5">
              <img v-for="image in images" :src="image" :class="{ active: image === images[currentImage] }" alt="">
            </div>
            <!-- /carusel -->
            <div class="next d-flex align-items-center">
              <button @click="nextImage()">NEXT</button>
            </div>
            <!-- /next -->
          </div>
        </div>
      </div>
      <!-- /col-12 -->
    </div>
    <!-- /row -->
  </div>
  <!-- /container-fluid -->
</template>


<style lang="scss" scoped>
@import "../assets/scss/partials/variables";

.row {
  background-repeat: no-repeat;
  display: flex;
  justify-content: center;
  background-position-x: 50%;
}

.advance {
  width: 100%;

  .prev button,
  .next button {
    padding: 10px;
    background-color: $header_text_color;
    color: $header_btn;
    border: none;
    border-radius: 50%;
    height: 40px;
    margin-left: -10px;
    margin-right: -10px;
    cursor: pointer;
    transition: all 0.2s ease-in-out;
  }

  .prev button:hover,
  .next button:hover {
    background-color: $header_text_color;
    transform: scale(1.1);
  }

  .prev button:before,
  .next button:before {
    content: '';
    display: block;
    width: 10px;
    height: 10px;
    transform: rotate(45deg);
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
  }

  .prev button {
    transform: rotate(90deg);
  }

  .next button {
    transform: rotate(-90deg);
  }

  .prev button:before {
    right: 12px;
  }

  .next button:before {
    left: 12px;
  }

  .carousel {
    text-align: center;
    background-repeat: no-repeat;
    width: 50%;
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
</style>