<script>
import NavbarHeader from './NavbarHeader.vue';
export default {
  name: 'AppHeader',
  components: {
    NavbarHeader
  },

}
</script>
<template>
  <header>

    <NavbarHeader />
    <section class="d-flex justify-content-center">
      <div class="advance d-flex justify-content-between">
        <div class="prev d-flex align-items-center">
          <button>PREV</button>
        </div>
        <div class="carosel">
          <img height="400px" src="../assets/img/h3-rev-img-4.png" alt="">
        </div>
        <div class="next d-flex align-items-center">
          <button>NEXT</button>
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

    .prev button {
      padding: 10px;
      background-color: $header_text_color;
      color: $header_btn;
      border: none;
      border-radius: 50% 50% 0 0;
      writing-mode: vertical-rl;
      transform: rotate(90deg);
      height: 40px;
      margin-left: -8px;
    }

    .next button {
      padding: 10px;
      background-color: $header_text_color;
      color: $header_btn;
      border: none;
      border-radius: 50% 50% 0 0;
      writing-mode: vertical-rl;
      transform: rotate(-90deg);
      height: 40px;
      margin-right: -8px;
    }

    .carosel {
      text-align: center;
      background-image: url(../assets/img/h3-rev-img-5.png);
      background-repeat: no-repeat;
      width: 53%;
    }
  }




}
</style>