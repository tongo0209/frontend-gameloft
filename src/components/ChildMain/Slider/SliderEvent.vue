
<template>
  <div>
    <div class="navigation-wrapper">
      <div ref="slider" class="keen-slider">
        <div class="keen-slider__slide number-slide1">1</div>
        <div class="keen-slider__slide number-slide1">1</div>
        <div class="keen-slider__slide number-slide1">1</div>
        <div class="keen-slider__slide number-slide1">1</div>
        <div class="keen-slider__slide number-slide1">1</div>
        <div class="keen-slider__slide number-slide1">1</div>
        <div class="keen-slider__slide number-slide1">1</div>
        <div class="keen-slider__slide number-slide1">1</div>
        <div class="keen-slider__slide number-slide1">1</div>
        <div class="keen-slider__slide number-slide1">1</div>
        <div class="keen-slider__slide number-slide1">1</div>
        <div class="keen-slider__slide number-slide1">1</div>
        <div class="keen-slider__slide number-slide1">1</div>
        <div class="keen-slider__slide number-slide1">1</div>
        <div class="keen-slider__slide number-slide1">1</div>
      </div>
    </div>
    <div v-if="slider" class="dots">
      <button
        v-for="val in dotHelper"
        @click="slider.moveToSlideRelative(val)"
        :class="{ dot: true, active: current === val || current === val + 1 }"
        :key="val"
      ></button>
    </div>
  </div>
</template>

<script>
import "keen-slider/keen-slider.min.css";
import KeenSlider from "keen-slider";

export default {
  name: "Slider",
  computed: {
    dotHelper() {
      console.log(
        [...Array(this.slider.details().size).keys()].filter(
          (x, i) => i % 2 === 0
        )
      );
      return this.slider
        ? [...Array(this.slider.details().size).keys()].filter(
            (x, i) => i % 2 === 0
          )
        : [];
    },
  },
  data() {
    return {
      current: 1,
      slider: null,
    };
  },
  mounted() {
    this.slider = new KeenSlider(this.$refs.slider, {
      initial: this.current,
      slidesPerView: 5,
      slideChanged: (s) => {
        this.current = s.details().relativeSlide;
      },
    });
  },
  beforeDestroy() {
    if (this.slider) this.slider.destroy();
  },
};
</script>

<style scoped>
[class^="number-slide"],
[class*=" number-slide"] {
  display: flex;
  align-items: center;
  justify-content: center;
  font-size: 50px;
  color: #fff;
  font-weight: 500;
  height: 400px;
}

.number-slide1 {
  margin: 0 1.5rem;
  border-radius: 10px;
  background: rgb(64, 175, 255);
  background: linear-gradient(
    128deg,
    rgba(64, 175, 255, 1) 0%,
    rgba(63, 97, 255, 1) 100%
  );
  width: 200px;
}
.number-slide1:hover {
  cursor: pointer;
  width: 220px;
  height: 400px;
}

.navigation-wrapper {
  position: relative;
}

.dots {
  display: flex;
  justify-content: center;
}

.dot {
  border: none;
  width: 20px;
  height: 20px;
  border: 3px solid #2699fb;
  background: transparent;
  border-radius: 50%;
  margin: 3rem 10px;
  padding: 5px;
  cursor: pointer;
}

.dot:focus {
  border: 3px solid #2699fb;
}

.dot.active {
  background: transparent;
  border: 3px solid #2699fb;
}

.arrow {
  width: 30px;
  height: 30px;
  position: absolute;
  top: 50%;
  transform: translateY(-50%);
  -webkit-transform: translateY(-50%);
  fill: #fff;
  cursor: pointer;
}
</style>



