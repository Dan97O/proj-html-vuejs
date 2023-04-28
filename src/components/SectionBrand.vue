<script>
export default {
  name: 'SectionBrand'
}
</script>
<template>
  <div class="container-fluid">
    <div class="row mt-2">
      <div class="background col-12 d-flex justify-content-center align-items-center py-5 p-0">
        <div class="d-none d-xxl-block">
          <img src="../assets/img/h1-clients-img-4.png" alt="">
        </div>
        <div class="d-none d-lg-block">
          <img src="../assets/img/h1-clients-img-3.png" alt="">
        </div>
        <div class="d-none d-md-block">
          <img src="../assets/img/h1-clients-img-1.png" alt="">
        </div>
        <div class="d-none d-sm-block">
          <img src="../assets/img/h1-clients-img-2.png" alt="">
        </div>
        <div>
          <img src="../assets/img/h1-clients-img-5.png" alt="">
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

.background {
  background-color: $background_brand;
}
</style>