<script>
export default {
  name: 'SectionBackground'

}
</script>


<template>
  <div class="container-fluid p-0">
    <div class="row mt-2">
      <div class="col-1 p-0">
        <img class="img_top_left img-fluid" src="../assets/img/h3-background-img.jpg" alt="">
      </div>
      <div class="col-10 p-0">
        <img class="img_top img-fluid" src="../assets/img/h3-background-img.jpg" alt="">
      </div>
      <div class="col-1 p-0">
        <img class="img_top_right img-fluid" src="../assets/img/h3-background-img.jpg" alt="">
      </div>
    </div>
    <!-- /row-top -->
    <div class="row">
      <div class="col-1 p-0">
        <img class="img_mid_left img-fluid" src="../assets/img/h3-background-img.jpg" alt="">
      </div>
      <!-- /.col-1 -->
      <div class="col-10 p-0 position-relative">
        <img class="img_mid img-fluid" src="../assets/img/h3-background-img.jpg" alt="">
        <div class="my_container">
          <h2>GO AHEAD AND BUILD YOUR OWN PIZZA WE WON'T JUDGE</h2>
        </div>
      </div>
      <!-- /.col-10 -->
      <div class="col-1 p-0 position-relative">
        <img class="img_mid_right img-fluid " src="../assets/img/h3-background-img.jpg" alt="">
        <div class="container_pizza d-flex justify-content-end pe-5 w-100">
          <img class="pizza" src="../assets/svg/svg-4.svg" alt="">
        </div>


      </div>
      <!-- /.col-1 -->
    </div>
    <!-- /.row-center -->
    <div class="row">
      <div class="col-1 p-0">
        <img class="img_bottom_left img-fluid" src="../assets/img/h3-background-img.jpg" alt="">
      </div>
      <!-- /.col-1 -->
      <div class="col-10 p-0">
        <img class="img_bottom img-fluid" src="../assets/img/h3-background-img.jpg" alt="">
      </div>
      <!-- /.col-10 -->
      <div class="col-1 p-0">
        <img class="img_bottom_right img-fluid" src="../assets/img/h3-background-img.jpg" alt="">
      </div>
      <!-- /.col-1 -->
    </div>
    <!-- /.row-bottom -->
  </div>
  <!-- /container -->
</template>


<style lang="scss" scoped>
@import "../assets/scss/partials/variables";

.container-fluid {
  height: 450px;

  /* #region row-top */
  .img_top_left {
    height: 100px;
    width: 100%;
    object-fit: none;
    object-position: right bottom;
  }

  .img_top {
    height: 100px;
    width: 100%;
    object-fit: cover;
    object-position: bottom;
  }

  .img_top_right {
    height: 100px;
    width: 100%;
    object-fit: none;
    object-position: left bottom;
  }

  /* #endregion row-top */

  /* #region row-middle */

  .img_mid_left {
    height: 250px;
    width: 100%;
    object-fit: none;
    object-position: right top;
  }

  .img_mid {
    height: 250px;
    width: 100%;
    object-fit: cover;
    object-position: top;
  }

  .my_container {
    position: absolute;
    top: -25px;
    left: 300px;
    width: 25%;

    h2 {
      font-size: 50px;
      color: $header_text_color;
    }
  }

  .img_mid_right {
    height: 250px;
    width: 100%;
    object-fit: none;
    object-position: left top;
  }

  .container_pizza {
    position: absolute;
    bottom: 40px;
  }

  .pizza {
    bottom: 0;
    border-radius: 50%;
    background-color: $circle_pizza;
    padding: 6px;
    aspect-ratio: 1/1;
    height: 36px;
  }

  /* #endregion row-middle */

  /* #region row-bottom */
  .img_bottom_left {
    height: 100px;
    width: 100%;
    object-fit: none;
    object-position: center right;
  }

  .img_bottom {
    height: 100px;
    width: 100%;
    object-fit: cover;
    object-position: center right;
  }

  .img_bottom_right {
    height: 100px;
    width: 100%;
    object-fit: none;
    object-position: left center;
  }

  /* #endregion row-middle */

}
</style>