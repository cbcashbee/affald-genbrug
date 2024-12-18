<script>
import '../assets/style/slider.scss';

export default {
  props: {
    slides: {
      type: Array,
      required: true,
    },
  },
  data() {
    return {
      currentIndex: 0,
    };
  },
  methods: {
    nextSlide() {
      this.currentIndex =
        (this.currentIndex + 1) % this.slides.length;
    },
    prevSlide() {
      this.currentIndex =
        (this.currentIndex - 1 + this.slides.length) % this.slides.length;
    },
    goToSlide(index) {
      this.currentIndex = index;
    },
  },
};
</script>

<template>
  <div class="slideshow">
    <div
      class="slides"
      :style="{ transform: `translateX(-${currentIndex * 100}%)` }"
    >
      <div class="slide" v-for="(slide, index) in slides" :key="index">
        <img :src="slide" :alt="'Slide ' + (index + 1)" />
      </div>
    </div>
    <button @click="prevSlide" class="prev">❮</button>
    <button @click="nextSlide" class="next">❯</button>
    <div class="indicators">
      <span
        v-for="(slide, index) in slides"
        :key="'indicator-' + index"
        :class="{ active: index === currentIndex }"
        @click="goToSlide(index)"
      ></span>
    </div>
  </div>
</template>