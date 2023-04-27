<script>
export default {
  name: 'SectionTeams'
}
</script>


<template>
  <div class="container-fluid mt-2">
    <div class="row">
      <div class="col-3 p-0">
        <img class="img-fluid" src="../assets/img/h1-team-1a-700x700.jpg" alt="">
        <div class="text">
          <span class="m-0"> <strong>FRANK BAILEY</strong> </span> <br>
          <span>Kitchen Porter</span> <br>
          <span>
            <i class="fa-brands fa-twitter fa-bounce px-1"></i>
            <i class="fa-brands fa-facebook fa-fade px-1"></i>
            <i class="fa-brands fa-instagram fa-beat-fade px-1"></i>
          </span>
        </div>
      </div>
      <!-- /.col-3 -->
      <div class="col-3 p-0">
        <img class="img-fluid" src="../assets/img/h1-team-2a.jpg" alt="">
        <div class="text">
          <span class="m-0"> <strong>FRANK BAILEY</strong> </span> <br>
          <span>Kitchen Porter</span> <br>
          <span>
            <i class="fa-brands fa-twitter fa-bounce px-1"></i>
            <i class="fa-brands fa-facebook fa-fade px-1"></i>
            <i class="fa-brands fa-instagram fa-beat-fade px-1"></i>
          </span>
        </div>
      </div>
      <!-- /.col-3 -->
      <div class="col-3 p-0">
        <img class="img-fluid" src="../assets/img/h1-team-4a.jpg" alt="">
        <div class="text">
          <span class="m-0"> <strong>FRANK BAILEY</strong> </span> <br>
          <span>Kitchen Porter</span> <br>
          <span>
            <i class="fa-brands fa-twitter fa-bounce px-1"></i>
            <i class="fa-brands fa-facebook fa-fade px-1"></i>
            <i class="fa-brands fa-instagram fa-beat-fade px-1"></i>
          </span>
        </div>
      </div>
      <!-- /.col-3 -->
      <div class="col-3 p-0 position-relative">
        <img class="img-fluid" src="../assets/img/h1-team-3a.jpg" alt="">
        <div class="text">
          <span class="m-0"> <strong>FRANK BAILEY</strong> </span> <br>
          <span>Kitchen Porter</span> <br>
          <span>
            <i class="fa-brands fa-twitter fa-bounce px-1"></i>
            <i class="fa-brands fa-facebook fa-fade px-1"></i>
            <i class="fa-brands fa-instagram fa-beat-fade px-1"></i>
          </span>
        </div>
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


.col-3 {
  position: relative;
  cursor: pointer;

  .text {
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
    text-align: center;
    border: 20px solid white;
    opacity: 0;
    background-color: red;
    color: white;
    padding: 10px;
    height: 100%;
    width: 100%;
    transition: opacity 0.5s ease-in-out;
  }

  &:hover .text {
    opacity: 1;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
  }

  img {
    transition: opacity 0.5s ease-in-out;
  }

  &:hover img {
    opacity: 0;
  }
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