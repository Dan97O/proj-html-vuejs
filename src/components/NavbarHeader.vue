<script>
export default {
  name: 'NavbarHeader',
  props: {
    pages: Array,
    links: Array
  },
  methods: {
    scrollToSectionTable() {
      const sectionTable = document.getElementById("sectionTable");
      sectionTable.scrollIntoView({ behavior: "smooth" });
    },
    scrollToMenu() {
      const sectionMenu = document.getElementById("sectionMenu");
      sectionMenu.scrollIntoView({ behavior: "smooth" });
    },
  },
}
</script>


<template>
  <div class="container-fluid">
    <div class="row">
      <div class="col-12">
        <nav class="d-flex justify-content-center align-items-center py-4">
          <button @click="scrollToSectionTable()" class="btn rounded-0 me-5">ORDER ONLINE</button>
          <ul class="d-flex gap-3 m-0">
            <li>
              <a class="d-flex align-items-center" :href="pages[0].url"><img style="height: 13px;" class="img-fluid me-2"
                  src="../assets/svg/svg-0.svg" :alt="pages[0].title"> {{ pages[0].title }}</a>
            </li>
            <li><a :href="pages[1].url"> {{ pages[1].title }}</a></li>
            <li><button @click="scrollToMenu()" class="p-0 border-0 bg-transparent">{{ pages[2].title }}</button></li>
          </ul>
          <!-- /ul pages -->
          <img class="logo mx-3" src="../assets/img/h5-logo-divided-header.png" alt="">
          <ul class="d-flex gap-3 m-0 me-5 p-0">
            <li v-for="link in links">
              <a :href="link.url">{{ link.title }}</a>
            </li>
          </ul>
          <!-- /ul links -->
          <ul class="d-flex gap-3 m-0">
            <li>
              <a class="d-flex" href="#"><img class="img-fluid me-2" src="../assets/svg/svg-1.svg" alt=""> CART</a>
            </li>
            <li>
              <a class="d-flex" href="#"><i class="fa-solid fa-magnifying-glass fa-rotate-90 me-2"></i> SEARCH</a>
            </li>
          </ul>
          <!-- /ul cart and search -->
        </nav>
        <!-- /nav -->
      </div>
      <!-- /col-12 -->
    </div>
    <!-- /row -->
  </div>
  <!-- /container-fluid -->
</template>


<style lang="scss" scoped>
@import "../assets/scss/partials/variables";

a:hover {
  color: $text_footer ;
}


nav {
  flex-wrap: wrap;

  button {
    background-color: $header_btn;
    color: $header_text_color;

    &:hover {
      background-color: $header_btn;
      color: $text_footer;
    }
  }

  ul {
    list-style: none;

    a {
      text-decoration: none;
      color: $header_text_color;

      img {
        color: white;
        background-color: white;
        filter: invert(0.9);
      }
    }
  }

  .logo {
    height: 130px;
    cursor: pointer;
  }
}
</style>