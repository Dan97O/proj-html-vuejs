<script>
export default {

}
</script>
<template>
  <header>

    <nav class="d-flex justify-content-center align-items-center py-4">
      <button class="btn rounded-0 me-5">ORDER ONLINE</button>
      <ul class="d-flex gap-3 m-0">
        <li>
          <a class="d-flex align-items-center" href="#"><img style="height: 13px;" class="img-fluid me-2"
              src="../assets/svg/svg-0.svg" alt=""> HOME</a>
        </li>
        <li><a href="#">PAGES</a></li>
        <li><a href="#">MENU</a></li>
      </ul>
      <img class="logo mx-3" src="../assets/img/h5-logo-divided-header.png" alt="">
      <ul class="d-flex gap-3 m-0 me-5 p-0">
        <li><a href="#">EVENT</a></li>
        <li><a href="#">BLOG</a></li>
        <li><a href="#">LANDING</a></li>
      </ul>
      <ul class="d-flex gap-3 m-0">
        <li>
          <a class="d-flex" href="#"><img class="img-fluid me-2" src="../assets/svg/svg-1.svg" alt=""> CART</a>
        </li>
        <li>
          <a class="d-flex" href="#"><i class="fa-solid fa-magnifying-glass fa-rotate-90 me-2"></i> SEARCH</a>
        </li>
      </ul>
    </nav>
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


  nav {
    display: flex;
    justify-content: center;

    button {
      background-color: $header_btn;
      color: $header_text_color;
    }

    ul {
      list-style: none;

      a {
        text-decoration: none;
        color: $header_text_color;


        img {
          color: white;
          background-color: white;
          filter: invert(1);
        }
      }
    }

    .logo {
      height: 130px;
    }
  }

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