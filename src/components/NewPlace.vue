<script>
export default {

}
</script>

<template>
  <div class="container-fluid p-0">
    <div class="row mt-2">
      <div class="col-3 p-0 pe-2">
        <a href="#"><img class="img-fluid" src="../assets/img/h3-img-1.jpg" alt=""></a>
        <div class="eyes">
          <i class="fa-solid fa-eye fa-shake"></i>
        </div>
      </div>
      <!-- /.col-3 -->
      <div class="col-3 p-0 pe-2">
        <a href="#"><img class="img-fluid" src="../assets/img/h3-img-2.jpg" alt=""></a>
        <div class="eyes">
          <i class="fa-solid fa-eye fa-shake"></i>
        </div>
      </div>
      <!-- /.col-3 -->
      <div class="col-3 p-0 pe-2">
        <a href="#"><img class="img-fluid" src="../assets/img/h3-img-3.jpg" alt=""></a>
        <div class="eyes">
          <i class="fa-solid fa-eye fa-shake"></i>
        </div>
      </div>
      <!-- /.col-3 -->
      <div class="col-3 p-0 pe-2">
        <a href="#"><img class="img-fluid" src="../assets/img/h3-img-4.jpg" alt=""></a>
        <div class="eyes">
          <i class="fa-solid fa-eye fa-shake"></i>
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

.col-3 {
  position: relative;

  &:hover {
    img {
      filter: opacity(0);
    }

    .eyes {
      display: flex;
      align-items: center;
      justify-content: center;

    }
  }
}

img {
  transition: filter 0.3s ease-out;
  max-width: 100%;
  height: auto;
}

.eyes {
  color: $header_text_color;
  background-color: $text_red;
  padding: 15px;
  aspect-ratio: 1/1;
  border-radius: 50%;
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  display: none;
}
</style>