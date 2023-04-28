<script>
export default {
  name: 'SectionPizza'
}
</script>


<template>
  <div id="sectionMenu" class="container-fluid ">
    <div class="row">
      <div class="col-12 p-0 d-flex justify-content-center align-items-center py-5">
        <div class="pizze text-center">
          <img src="../assets/img/h3-product-img-1a-100x100.png" alt="">
          <br>
          <span class="name_pizza">BISMARCK</span> <br>
          <span class="first_price text-decoration-line-through">$5.00</span> <span class="second_price">$30.00</span>
        </div>
        <div class="pizze text-center">
          <img src="../assets/img/h3-product-img-2a-150x150.png" alt="">
          <br>
          <span class="name_pizza">FIORI DI ZUCCA</span> <br>
          <span class="second_price">$7.00 - $50.00</span>
        </div>
        <div class="pizze text-center position-relative ">
          <img src="../assets/img/h3-product-img-3a-150x150.png" alt="">
          <span class="sold">SOLD</span>
          <br>
          <span class="name_pizza">VALDOSTANA</span> <br>
          <span class="second_price">$55.00</span>
        </div>
        <div class="pizze text-center">
          <img src="../assets/img/h3-product-img-4a-150x150.png" alt="">
          <br>
          <span class="name_pizza">PIZZA TARTUFATA</span> <br>
          <span class="second_price">$45.00</span>
        </div>
        <div class="pizze text-center">
          <img src="../assets/img/h3-product-img-5a-150x150.png" alt="">
          <br>
          <span class="name_pizza">FRANCESCANA</span> <br>
          <span class="second_price">$25.00</span>
        </div>
        <div class="pizze text-center">
          <img src="../assets/img/h3-product-img-6a-100x100.png" alt="">
          <br>
          <span class="name_pizza">CAMPAGNOLA</span> <br>
          <span class="second_price">$50.00 - $95.00</span>
        </div>
      </div>
      <!-- /.col-12 -->
    </div>
    <!-- /.row -->
  </div>
  <!-- /.container-fluid -->
</template>


<style lang="scss" scoped>
@import "../assets/scss/partials/variables";

img {
  margin: 0 7rem;
  height: 150px;
}

.name_pizza {
  color: $name_pizza;
}

.first_price {
  color: $first_price;
}

.second_price {
  color: $header_btn;
}

.sold {
  position: absolute;
  font-size: 8px;
  right: 0px;
  top: 12px;
  aspect-ratio: 1;
  display: flex;
  align-items: center;
  justify-content: center;
  right: 102px;
  color: $header_text_color;
  background-color: $header_btn;
  border-radius: 50%;
  padding: 10px;
}
</style>