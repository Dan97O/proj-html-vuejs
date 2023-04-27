<script>
export default {
  name: 'SectionTable',
}
</script>


<template>
  <div class="container-fluid p-0 mt-2">
    <div class="row h-100">
      <div class="col-12 p-0 d-flex justify-content-center align-items-center">
        <div class=" position-relative">
          <select class="form-select form-select-sm me-3" aria-label=".form-select-sm example">
            <option selected>Select people</option>
            <option value="1">1</option>
            <option value="2">2</option>
            <option value="3">3</option>
            <option value="4">4</option>
            <option value="5">5</option>
            <option value="6">6</option>
            <option value="7">7</option>
            <option value="8">8</option>
            <option value="9">9</option>
            <option value="10">10</option>
          </select>
          <!-- /select people -->
          <span class="powered">*Powered by OpenTable</span>
        </div>
        <span>FOR</span>
        <select class="form-select form-select-sm mx-3" aria-label=".form-select-sm example">
          <option value="">Select date</option>
          <option value="28-04-2023">28 April 2023</option>
          <option value="29-04-2023">29 April 2023</option>
          <option value="30-04-2023">30 April 2023</option>
          <option value="01-05-2023">1 May 2023</option>
          <option value="02-05-2023">2 May 2023</option>
          <option value="03-05-2023">3 May 2023</option>
          <option value="04-05-2023">4 May 2023</option>
          <option value="05-05-2023">5 May 2023</option>
          <option value="06-05-2023">6 May 2023</option>
        </select>
        <!-- /select date -->
        <span>AT</span>
        <select class="form-select form-select-sm mx-3" aria-label=".form-select-sm example">
          <option value="">Select time</option>
          <option value="17:00">5:00 PM</option>
          <option value="18:00">6:00 PM</option>
          <option value="19:00">7:00 PM</option>
          <option value="20:00">8:00 PM</option>
          <option value="21:00">9:00 PM</option>
          <option value="22:00">10:00 PM</option>
          <option value="23:00">11:00 PM</option>
        </select>
        <!-- /select time -->
        <button class="btn rounded-0 ms-5">BOOK A TABLE</button>
      </div>
      <!-- /.col-12 -->
    </div>
    <!-- /.row -->
  </div>
  <!-- /.container-fluid -->
</template>


<style lang="scss" scoped>
@import "../assets/scss/partials/variables";

.container-fluid {
  background-image: url('../assets/img/h3-background-img-3.jpg');
  color: $header_text_color;

  .row {
    padding: 5rem 0;
  }

  select {
    width: 200px;
    height: 50px;
  }

  button {
    background-color: $header_btn;
    color: $header_text_color;
    height: 50px;
    width: 200px;
    font-size: 12px;
  }

  .powered {
    position: absolute;
    top: 55px;
    left: 0px;
    font-size: 12px;
  }

}
</style>