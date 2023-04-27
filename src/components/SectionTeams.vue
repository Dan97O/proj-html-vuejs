<script>
export default {
  name: 'SectionTeams'
}
</script>


<template>
  <div class="container-fluid p-0 mt-2">
    <div class="row">
      <div class="col-3 p-0">
        <img class="img-fluid" src="../assets/img/h1-team-1a-700x700.jpg" alt="">
      </div>
      <!-- /.col-3 -->
      <div class="col-3 p-0">
        <img class="img-fluid" src="../assets/img/h1-team-2a.jpg" alt="">
      </div>
      <!-- /.col-3 -->
      <div class="col-3 p-0">
        <img class="img-fluid" src="../assets/img/h1-team-4a.jpg" alt="">
      </div>
      <!-- /.col-3 -->
      <div class="col-3 p-0 position-relative">
        <img class="img-fluid" src="../assets/img/h1-team-3a.jpg" alt="">
        <div class="container_pizza d-flex justify-content-end pe-5 w-100">
          <img class="pizza" src="../assets/svg/svg-4.svg" alt="">
        </div>
      </div>
      <!-- /.col-3 -->
    </div>
    <!-- /.row -->
  </div>
  <!-- /.container-fluid -->
</template>


<style lang="scss" scoped>
@import "../assets/scss/partials/variables";

.container_pizza {
  position: absolute;
  bottom: 40px;

  .pizza {
    border-radius: 50%;
    background-color: $circle_pizza;
    padding: 6px;
    aspect-ratio: 1/1;
    height: 36px;
  }
}
</style>