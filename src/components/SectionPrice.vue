<script>
export default {
  name: 'SectionPrice'

}
</script>


<template>
  <div class="container-fluid">
    <div class="row mt-2">
      <div class="col-6 p-0 position-relative">
        <img class="img-fluid" src="../assets/img/h1-img-4.jpg" alt="">
        <div class="special d-none d-lg-block">
          <img class="img-fluid" src="../assets/img/h1-img-7n.png" alt="">
        </div>
      </div>
      <!-- /.col-6 -->
      <div class="col-6 d-flex justify-content-center align-items-center flex-column">
        <div class="price">
          <h3>SPECIALS*</h3>
          <p>Lorem, ipsum dolor sit amet consectetur adipisicing elit. Corrupti, perspiciatis!</p>
          <div class="d-none d-sm-flex">
            <div>
              <h4 class="dollars">$10</h4>
            </div>
            <div class="ms-3">
              <h4>COMBO PICCOLO</h4>
              <span>Lorem ipsum, dolor sit amet consectetur adipisicing elit. Eius, explicabo.</span>
            </div>
          </div>
          <div class="mt-3 d-none d-md-flex">
            <div>
              <h4 class="dollars">$20</h4>
            </div>
            <div class="ms-3">
              <h4>COMBO MEZZO</h4>
              <span>Lorem ipsum, dolor sit amet consectetur adipisicing elit. Eius, explicabo.</span>
            </div>
          </div>
          <div class="mt-3 d-none d-xl-flex">
            <div>
              <h4 class="dollars">$30</h4>
            </div>
            <div class="ms-3">
              <h4>COMBO GRANDE</h4>
              <span>Lorem ipsum, dolor sit amet consectetur adipisicing elit. Eius, explicabo.</span>
            </div>
          </div>
        </div>
        <div class="d-flex justify-content-end pe-5 w-100">
          <img class="pizza" src="../assets/svg/svg-4.svg" alt="">
        </div>
      </div>
      <!-- /.col-6 -->
    </div>
    <!-- /.row -->
  </div>
  <!-- /.container-fluid -->
</template>


<style lang="scss" scoped>
@import "../assets/scss/partials/variables";

.special {
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
}

.price {
  width: 50%;

  .dollars {
    color: $header_btn;
  }
}

.pizza {
  border-radius: 50%;
  background-color: $circle_pizza;
  padding: 6px;
  aspect-ratio: 1/1;
  height: 36px;
}
</style>