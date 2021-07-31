
<template>
  <div>
    <div class="navigation-wrapper">
      <div ref="slider" class="keen-slider">
        <div class="keen-slider__slide number-slide1">
          <img src="../../assets/carousel/Carousel-1.png" alt="" />
          <div class="short__title">Short title</div>
        </div>
        <div class="keen-slider__slide number-slide2">
          <img src="../../assets/carousel/Carousel-2.png" alt="" />
          <div class="short__title">Short title</div>
        </div>
        <div class="keen-slider__slide number-slide3">
          <img src="../../assets/carousel/Carousel-3.png" alt="" />
          <div class="short__title">Short title</div>
        </div>
        <div class="keen-slider__slide number-slide4">
          <img src="../../assets/carousel/Carousel-4.png" alt="" />
          <div class="short__title">Short title</div>
        </div>
        <div class="keen-slider__slide number-slide5">
          <img src="../../assets/carousel/Carousel-5.png" alt="" />
          <div class="short__title">Short title</div>
        </div>
        <div class="keen-slider__slide number-slide6">
          <img src="../../assets/carousel/Carousel-6.png" alt="" />
          <div class="short__title">Short title</div>
        </div>
        <div class="keen-slider__slide number-slide7">
          <img src="../../assets/carousel/Carousel-8.png" alt="" />
          <div class="short__title">Short title</div>
        </div>
        <div class="keen-slider__slide number-slide7">
          <img src="../../assets/carousel/Carousel-8.png" alt="" />
          <div class="short__title">Short title</div>
        </div>
        <div class="keen-slider__slide number-slide7">
          <img src="../../assets/carousel/Carousel-8.png" alt="" />
          <div class="short__title">Short title</div>
        </div>
        <div class="keen-slider__slide number-slide7">
          <img src="../../assets/carousel/Carousel-8.png" alt="" />
          <div class="short__title">Short title</div>
        </div>
      </div>

      <svg
        @click="slider.prev()"
        :class="{
          arrow: true,
          'arrow--left': true,
          'arrow--disabled': current === 0,
        }"
        xmlns="http://www.w3.org/2000/svg"
        viewBox="0 0 24 24"
      >
        <path
          d="M11.354 1.646a.5.5 0 0 1 0 .708L5.707 8l5.647 5.646a.5.5 0 0 1-.708.708l-6-6a.5.5 0 0 1 0-.708l6-6a.5.5 0 0 1 .708 0z"
        />
      </svg>
      <svg
        v-if="slider"
        @click="slider.next()"
        :class="{
          arrow: true,
          'arrow--right': true,
          'arrow--disabled': current === dotHelper[dotHelper.length - 1],
        }"
        xmlns="http://www.w3.org/2000/svg"
        viewBox="0 0 24 24"
      >
        <path
          d="M4.646 1.646a.5.5 0 0 1 .708 0l6 6a.5.5 0 0 1 0 .708l-6 6a.5.5 0 0 1-.708-.708L10.293 8 4.646 2.354a.5.5 0 0 1 0-.708z"
        />
      </svg>
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
  color: #fff;
}
.short__title {
  color: #2699fb;
  margin-left: 1rem;
  font-size: 15px;
}
.keen-slider {
  padding-left: 3rem;
  padding-right: 0rem;
}
img {
  width: 100px;
  height: 100px;
  padding: 5px;
  border-radius: 50%;
}
img:hover {
  border: 2px solid #2699fb;
  cursor: pointer;
}

.navigation-wrapper {
  position: relative;
}

.arrow {
  width: 60px;
  height: 60px;
  position: absolute;
  top: 50%;
  transform: translateY(-50%);
  -webkit-transform: translateY(-50%);
  fill: #2699fb;
  cursor: pointer;
}

.arrow--left {
  left: 5px;
  background-color: transparent;
}

.arrow--right {
  left: auto;
  right: 5px;
  background-color: transparent;
}

.arrow--disabled {
  fill: #d5ecff;
  background-color: transparent;
}
</style>



