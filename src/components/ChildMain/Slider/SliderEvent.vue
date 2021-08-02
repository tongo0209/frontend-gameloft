
<template>
  <div>
    <div class="navigation-wrapper">
      <div ref="slider" class="keen-slider">
        <div class="keen-slider__slide number-slide1">
          <div class="main">
            <div class="image">
              <img src="../../../assets/icon/icon-hotposter.png" alt="" />
            </div>
            <div class="title">Short title here</div>
          </div>
        </div>
        <div class="keen-slider__slide number-slide1">
          <div class="main">
            <div class="image">
              <img src="../../../assets/icon/icon-hotposter.png" alt="" />
            </div>
            <div class="title">Short title here</div>
          </div>
        </div>
        <div class="keen-slider__slide number-slide1">
          <div class="main">
            <div class="image">
              <img src="../../../assets/icon/icon-hotposter.png" alt="" />
            </div>
            <div class="title">Short title here</div>
          </div>
        </div>
        <div class="keen-slider__slide number-slide1">
          <div class="main">
            <div class="image">
              <img src="../../../assets/icon/icon-hotposter.png" alt="" />
            </div>
            <div class="title">Short title here</div>
          </div>
        </div>
        <div class="keen-slider__slide number-slide1">
          <div class="main">
            <div class="image">
              <img src="../../../assets/icon/icon-hotposter.png" alt="" />
            </div>
            <div class="title">Short title here</div>
          </div>
        </div>
        <div class="keen-slider__slide number-slide1">
          <div class="main">
            <div class="image">
              <img src="../../../assets/icon/icon-hotposter.png" alt="" />
            </div>
            <div class="title">Short title here</div>
          </div>
        </div>
        <div class="keen-slider__slide number-slide1">
          <div class="main">
            <div class="image">
              <img src="../../../assets/icon/icon-hotposter.png" alt="" />
            </div>
            <div class="title">Short title here</div>
          </div>
        </div>
        <div class="keen-slider__slide number-slide1">
          <div class="main">
            <div class="image">
              <img src="../../../assets/icon/icon-hotposter.png" alt="" />
            </div>
            <div class="title">Short title here</div>
          </div>
        </div>
        <div class="keen-slider__slide number-slide1">
          <div class="main">
            <div class="image">
              <img src="../../../assets/icon/icon-hotposter.png" alt="" />
            </div>
            <div class="title">Short title here</div>
          </div>
        </div>
      </div>
    </div>
    <div v-if="slider" class="dots">
      <button
        v-for="val in dotHelper"
        @click="slider.moveToSlideRelative(val)"
        :class="{
          spin: true,
          cirle: true,
          active: current === val || current === val + 1,
        }"
        :key="val"
      >
        {{ val + 1 }}
      </button>
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
      return this.slider
        ? [...Array(this.slider.details().size).keys()].filter(
            (x, i) => i % 1 === 0
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
  background: linear-gradient(
    180deg,
    rgba(36, 153, 251, 1) 0%,
    rgba(36, 153, 251, 1) 50%,
    rgba(0, 0, 0, 1) 100%
  );
  min-width: 300px !important;
  max-width: 300px !important;
}
.number-slide1:hover {
  transition: min-width 0.3s ease, max-width 0.3s ease;
  min-width: 330px !important;
  max-width: 330px !important;
  cursor: pointer;
}
.main {
  display: flex;
  flex-direction: column;
  align-items: center;
  margin: 0 1rem;
}
.main .image {
  margin-top: 2rem;
}
.main .image img {
  width: 150px;
}
.main .title {
  font-size: 35px;
  margin-top: 8rem;
  font-weight: 700;
  text-transform: uppercase;
}
.navigation-wrapper {
  position: relative;
}

.dots {
  display: flex;
  justify-content: center;
  margin-top: 3rem;
}
button {
  background: none;
  border: 0;
  box-sizing: border-box;
  margin: 1em;
  padding: 1em 2em;
  color: #2699fb;
  font-size: inherit;
  font-weight: 700;
  position: relative;
  vertical-align: middle;
}
button::before,
button::after {
  box-sizing: inherit;
  content: "";
  position: absolute;
  width: 100%;
  height: 100%;
}
.spin {
  width: 2rem;
  height: 2rem;
  padding: 0;
  display: flex;
  font-weight: 300;
  justify-content: center;
  align-items: center;
  border-radius: 50%;
}
.spin:hover {
  color: #2699fb;
}
.spin::before,
.spin::after {
  top: 0;
  left: 0;
}
.spin::before {
  border: 3px solid transparent;
  border-radius: 50%;
}
.spin:hover::before {
  border-top-color: #e6f4ff;
  border-right-color: #2699fb;
  border-radius: 50%;
  transform: rotate(-45deg);
  border-bottom-color: #e6f4ff;
  transition: border-top-color 0.15s linear,
    border-right-color 0.15s linear 0.1s, border-bottom-color 0.15s linear 0.2s;
}
.spin:focus::before {
  border-top-color: #e6f4ff;
  border-right-color: #2699fb;
  border-radius: 50%;
  transform: rotate(-45deg);
  border-bottom-color: #e6f4ff;
}
.spin:active::before {
  border-top-color: #e6f4ff;
  border-right-color: #2699fb;
  border-radius: 50%;
  transform: rotate(-45deg);
  border-bottom-color: #e6f4ff;
}
.spin::after {
  border: 0 solid transparent;
  border-radius: 50%;
}
.spin:hover::after {
  border-top: 3px solid #e6f4ff;
  border-left-width: 3px;
  border-right-width: 3px;
  transform: rotate(225deg);
  transition: transform 0.4s linear 0s, border-left-width 0s linear 0.35s;
}
.spin:focus::after {
  border-top: 3px solid #e6f4ff;
  border-left-width: 3px;
  border-right-width: 3px;
  transform: rotate(225deg);
}
.spin:active::after {
  border-top: 3px solid #e6f4ff;
  border-left-width: 3px;
  border-right-width: 3px;
  transform: rotate(225deg);
}

@media only screen and (max-width: 430px) {
  .dots {
    display: none;
  }
  [class^="number-slide"],
  [class*=" number-slide"] {
    height: 350px;
  }
  .number-slide1 {
    min-width: 250px !important;
    max-width: 250px !important;
  }
}
</style>



