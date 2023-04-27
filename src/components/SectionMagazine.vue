<script>
export default {
  name: 'SectionMagazine'
}
</script>


<template>
  <div class="container-fluid">
    <div class="row mt-2 background">
      <div class="col-1 p-0 d-flex align-items-center">
        <div class="prev">
          <button>PREV</button>
        </div>
      </div>
      <div class="col-10 p-0 d-flex justify-content-center py-5">
        <div class="comments">
          <h1><i class="fa-solid fa-quote-left fa-beat"></i></h1>
          <h4>"FORGET THE PIZZA SHOPS, THIS HIDDEN SPOT MAKES THE BEST NEW YORK-STYLE PIZZA SLICE IN NAPLES"</h4>
          <span class="magazine">WASHINGTON POST 2018</span> <br>
          <div class="circle mt-3">
            <span class="me-1 ">
              <i class="fa-solid fa-circle fa-fade"></i>
            </span>
            <span class="me-1">
              <i class="fa-regular fa-circle"></i>
            </span>
            <span>
              <i class="fa-regular fa-circle"></i>
            </span>
          </div>
        </div>
      </div>
      <div class="col-1 p-0 d-flex align-items-end justify-content-center flex-column">
        <div class="next ">
          <button>NEXT</button>
        </div>
      </div>
      <div class="d-flex justify-content-end pe-5">
        <img src="../assets/svg/svg-4.svg" alt="">
      </div>
    </div>
    <!-- /.row -->
  </div>
  <!-- /.container-fluid -->
</template>


<style lang="scss" scoped>
@import "../assets/scss/partials/variables";

.prev button,
.next button {
  padding: 10px;
  background-color: $header_text_color;
  color: $header_btn;
  border: none;
  border-radius: 50%;
  height: 40px;
  margin-left: -10px;
  margin-right: -10px;
  cursor: pointer;
  transition: all 0.2s ease-in-out;
}

.prev button:hover,
.next button:hover {
  background-color: $header_text_color;
  transform: scale(1.1);
}

.prev button:before,
.next button:before {
  content: '';
  display: block;
  width: 10px;
  height: 10px;
  transform: rotate(45deg);
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
}

.prev button {
  transform: rotate(90deg);
}

.next button {
  transform: rotate(-90deg);
}

.prev button:before {
  right: 12px;
}

.next button:before {
  left: 12px;
}

.background {
  background-image: url(../assets/img/h3-testimonials-bckgrnd.jpg);
  padding: 5rem 0;
}

.comments {
  width: 50%;
  text-align: center;

  h1 {
    color: $text_quote;
  }

  .magazine {
    color: $header_btn;
  }

  .circle {
    span {
      color: $text_quote;
      font-size: 8px;
    }
  }
}
</style>