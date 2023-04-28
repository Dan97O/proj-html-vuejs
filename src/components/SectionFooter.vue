<script>
export default {
  name: 'SectionFooter',
  props: {
    restaurants: Array,
    working: Array
  },

}
</script>


<template>
  <div id="landing" class="container-fluid mt-2">
    <div class="row">
      <div class="col-6 p-0">
        <div class="row">
          <div class="col-4 d-none d-sm-block">
            <h5 class="pt-5 ps-4">FIND OUR RESTAURANTS</h5>
            <ul class="p-0 ps-4 d-none d-xl-block" v-for="restaurant in restaurants">
              <li>{{ restaurant.address }}</li>
              <li>{{ restaurant.city }}</li>
              <li>{{ restaurant.phone }}</li>
            </ul>
            <!-- /FIND OUR RESTAURANTS -->
            <div class="ps-4 pt-5">
              <span class="heart">
                Created with &hearts; by <span class="qode">Qode Interactive</span>
              </span>
              <!-- /created by -->
            </div>
          </div>
          <!-- /col-4 RESTAURANTS -->
          <div class="col-4">
            <h5 class="pt-5 d-none d-sm-block">WORKING HOURS</h5>
            <ul class="p-0" v-for="hours in working">
              <li class="day">{{ hours.day }}</li>
              <li v-bind:class="{ 'time': true, 'my_red': hours.time === 'Kitchen Closed' }">{{ hours.time }}</li>
            </ul>
            <div>
              <span class="day d-none d-sm-block">FOLLOW US:</span>
              <span class="icon d-none d-sm-block">
                <i class="fa-brands fa-twitter fa-bounce ps-2 px-1"></i>
                <i class="fa-brands fa-facebook fa-fade px-1"></i>
                <i class="fa-brands fa-instagram fa-beat-fade px-1"></i>
                <i class="fa-brands fa-linkedin fa-shake px-1"></i>
              </span>
              <!-- /icon -->
            </div>
          </div>
          <!-- /col-4 WORKING HOURS -->
          <div class="col-4 d-flex flex-column justify-content-between align-items-center d-none d-sm-flex">
            <h4 class="pt-5 pe-2 ps-2">THE DON PEPPE CREW FIRST AND FOREMOST VALUES AN AUTHENTIC, WELL BAKED SLICE OF
              PIZZA
            </h4>
            <img class="premium mb-5" src="../assets/img/natural-product-icon.png" alt="">
          </div>
          <!-- /col-4 -->
        </div>
        <!-- /row -->
      </div>
      <!-- /.col-6 -->
      <div class="col-6 p-0 position-relative">
        <img class="img-fluid img_footer" src="../assets/img/footer-img-1.jpg" alt="">
        <div class="container_pizza d-flex justify-content-end pe-5 w-100">
          <img class="pizza" src="../assets/svg/svg-4.svg" alt="">
        </div>
        <!-- /container_pizza -->
      </div>
      <!-- /.col-6 -->
    </div>
    <!-- /.row -->
  </div>
  <!-- /.container-fluid -->
</template>


<style lang="scss" scoped>
@import "../assets/scss/partials/variables";

li:hover {
  color: $header_text_color ;
  cursor: pointer;
}


.my_red {
  color: $text_red;
}

ul {
  list-style: none;
}

/* #region col-4 */
.col-4 {
  background-color: $background_dark;
  color: $text_footer;
  min-height: 584px;
  max-height: 584px;

  h5,
  .heart,
  .day {
    color: $line_dashed;
  }

  .qode {
    color: $text_green;
  }

  .icon {
    color: $header_text_color;
  }

  .premium {
    filter: invert(0.9);
    height: 100px;
    width: 100px;
    aspect-ratio: 1/1;
    color: $line_dashed !important;
  }

  h4 {
    color: $header_text_color;
  }

}

/* #endregion col-4 */
.img_footer {
  min-height: 584px;
  max-height: 584px;
  width: 100%;
  object-fit: cover;
}

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