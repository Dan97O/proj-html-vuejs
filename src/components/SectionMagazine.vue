<script>
export default {
  name: 'SectionMagazine',
  data() {
    return {
      comments: [
        {
          text: 'FORGET THE PIZZA SHOPS, THIS HIDDEN SPOT MAKES THE BEST NEW YORK-STYLE PIZZA SLICE IN NAPLES',
          source: 'WASHINGTON POST 2018',
        },
        {
          text: 'I WOULD HIGHLY RECOMMEND THIS PLACE FOR ANYONE WHO WANTS TO TRY AUTHENTIC ITALIAN PIZZA',
          source: 'NEW YORK TIMES 2019',
        },
        {
          text: 'THE PIZZA HERE IS OUT OF THIS WORLD. TRULY A GEM IN THE HEART OF NAPLES',
          source: 'NEW YORK POST 2020',
        },
      ],
      currentCommentIndex: 0,
    };
  },
  computed: {
    currentComment() {
      return this.comments[this.currentCommentIndex];
    },
  },
  methods: {
    prevComment() {
      this.currentCommentIndex = (this.currentCommentIndex - 1 + this.comments.length) % this.comments.length;
    },
    nextComment() {
      this.currentCommentIndex = (this.currentCommentIndex + 1) % this.comments.length;
    },
  },
}
</script>


<template>
  <div class="container-fluid">
    <div class="row mt-2 background">
      <div class="col-1 p-0 d-flex align-items-center">
        <div class="prev">
          <button @click="prevComment">PREV</button>
        </div>
      </div>
      <div class="col-10 p-0 d-flex justify-content-center py-5">
        <div class="comments">
          <h1><i class="fa-solid fa-quote-left fa-beat"></i></h1>
          <h4>{{ currentComment.text }}</h4>
          <span class="magazine">{{ currentComment.source }}</span> <br>
          <div class="circle mt-3">
            <span v-for="(comment, index) in comments" class="me-1">
              <i :class="`fa-${index === currentCommentIndex ? 'solid fa-fade' : 'regular'} fa-circle`"></i>
            </span>
          </div>
        </div>
      </div>
      <div class="col-1 p-0 d-flex align-items-end justify-content-center flex-column">
        <div class="next">
          <button @click="nextComment">NEXT</button>
        </div>
      </div>
      <div class="d-flex justify-content-end pe-5">
        <img src="../assets/svg/svg-4.svg" alt="">
      </div>
    </div>
  </div>
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