<script>
export default {
  name: 'SectionCalendar'
}
</script>

<template>
  <div id="calendar" class="container-fluid mt-2">
    <div class="row">
      <div class="col-6 col_left p-0 d-flex justify-content-start align-items-center flex-column">
        <div class="calendar pt-5">
          <span class="made">MADE WITH LOVE</span>
          <h4>DELISH PIZZA DEALS</h4>
          <div class="d-flex mt-4">
            <div>
              <h4 class="date_num m-0">02</h4>
              <span class="date">NOV</span>
            </div>
            <div class="ms-3 pb-3">
              <h5>TRADITIONAL NEAPOLITAN PIES IN KYOTO PIZZA MERCATO</h5>
              <span class="location"><i class="fa-solid fa-location-dot fa-fade"></i> 204 E. Pizzetta Tommaso </span>
            </div>
          </div>
          <!-- first date -->
          <hr>
          <div class="d-flex mt-4 d-none d-lg-flex">
            <div>
              <h4 class="date_num m-0">03</h4>
              <span class="date">NOV</span>
            </div>
            <div class="ms-3 pb-3">
              <h5>TERRAZZA PATIO DINING SPACE OPENING THIS WEEKEND</h5>
              <span class="location"><i class="fa-solid fa-location-dot fa-fade"></i> 204 E. Pizzetta Tommaso </span>
            </div>
          </div>
          <!-- second date -->
          <hr>
          <div class="d-flex mt-4 d-none d-xl-flex">
            <div>
              <h4 class="date_num m-0">05</h4>
              <span class="date">NOV</span>
            </div>
            <div class="ms-3 pb-3">
              <h5>SIENNA PRIVATE DINING ROOM WITH STEPHANE BRUNN</h5>
              <span class="location"><i class="fa-solid fa-location-dot fa-fade"></i> 204 E. Pizzetta Tommaso </span>
            </div>
          </div>
          <!-- third  date -->
        </div>
        <!-- /calendar -->
      </div>
      <!-- /.col-6 -->
      <div class="col-6 p-0 position-relative">
        <img class="img-fluid comics" src="../assets/img/h3-img-5a.jpg" alt="">
        <div class="carriage_top">
          <img src="../assets/svg/svg-10.svg" alt="">
        </div>
        <!-- carriage_top -->
        <div class="carriage">
          <img src="../assets/svg/svg-9.svg" alt="">
        </div>
        <!-- carriage -->
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

h5:hover {
  color: $text_footer ;
  cursor: pointer;
}

.col_left {
  background-color: $background_dark;
  background-image: url('../assets/img/costellazione.jpeg');

  height: 550px;
}

.calendar {
  width: 50%;
  color: white;

  .made {
    color: $text_red;
    font-size: 12px;

  }

  .date_num {
    color: $header_btn;
    font-size: 30px;
  }

  .location {
    color: $header_btn;
  }

  hr {
    border: 1px dashed $line_dashed;
  }
}

.comics {
  height: 650px;
  width: 100%;
  object-fit: cover;
}

.carriage_top {
  position: absolute;
  top: -40px;
  right: 0px;
  background-color: $header_btn;
  padding: 5px;

  img {
    height: 100%;
    height: 20px;
  }
}


.carriage {
  position: absolute;
  top: 0;
  right: 0px;
  background-color: $header_text_color;
  padding: 5px;

  img {
    height: 100%;
    height: 20px;
  }
}

.container_pizza {
  position: absolute;
  top: 30px;
  right: 0;
}

.pizza {
  border-radius: 50%;
  background-color: $circle_pizza;
  padding: 6px;
  aspect-ratio: 1/1;
  height: 36px;
}
</style>