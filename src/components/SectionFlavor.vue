<script>
export default {
  name: 'SectionFlavor'
}
</script>


<template>
  <div class="container-fluid p-0">
    <div class="row">
      <div class="col-12 d-flex justify-content-center align-items-center py-5 p-0">
        <div class="pizza_town ">
          <div>
            <span>CHOOSE YOUR FLAVOR</span>
          </div>
          <div>
            <h3> <strong>THE BEST PIZZA MENU IN TOWN</strong> </h3>
          </div>
          <div>
            <p>
              Lorem ipsum dolor sit amet consectetur adipisicing elit. Doloremque unde distinctio aut in delectus neque,
              nostrum deleniti nisi eligendi omnis.
            </p>
          </div>
        </div>
      </div>
      <!-- /.col-12 -->
      <div class="container_pizza d-flex justify-content-end pe-5 w-100">
        <img class="pizza" src="../assets/svg/svg-4.svg" alt="">
      </div>
    </div>
    <!-- /.row -->
  </div>
  <!-- /.container -->
</template>


<style lang="scss" scoped>
@import "../assets/scss/partials/variables";

.pizza_town {
  width: 50%;
  text-align: center;

  span {
    color: $header_btn;
    font-size: 14px;
  }
}

.container_pizza {
  margin-top: -4rem;

  .pizza {
    border-radius: 50%;
    background-color: $circle_pizza;
    padding: 6px;
    aspect-ratio: 1/1;
    height: 36px;
  }
}
</style>