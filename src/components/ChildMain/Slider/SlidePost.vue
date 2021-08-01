
<template>
  <div>
    <div class="navigation-wrapper">
      <div ref="slider" class="keen-slider">
        <div class="keen-slider__slide number-slide1">
          <div class="top__icon">
            <a href="#"
              ><img src="../../../assets/icon/facebook.png" alt="logo"
            /></a>
            <div class="share">
              <a href="#"
                ><img src="../../../assets/icon/share-black.png" alt="logo"
              /></a>
            </div>
          </div>
          <div class="bottom">
            Lorem ipsum dolor sit, amet consectetur adipisicing elit. Quisquam,
            dolorum! In, ad, deserunt cupiditate repellat explicabo
            maiorerepellat explicabo maiore
          </div>
        </div>
        <div class="keen-slider__slide number-slide1">
          <div class="top__icon">
            <a href="#"
              ><img src="../../../assets/icon/facebook.png" alt="logo"
            /></a>
            <div class="share">
              <a href="#"
                ><img src="../../../assets/icon/share-black.png" alt="logo"
              /></a>
            </div>
          </div>
          <div class="bottom">
            Lorem ipsum dolor sit, amet consectetur adipisicing elit. Quisquam,
            dolorum! In, ad, deserunt cupiditate repellat explicabo
            maiorerepellat explicabo maiore
          </div>
        </div>
        <div class="keen-slider__slide number-slide1">
          <div class="top__icon">
            <a href="#"
              ><img src="../../../assets/icon/facebook.png" alt="logo"
            /></a>
            <div class="share">
              <a href="#"
                ><img src="../../../assets/icon/share-black.png" alt="logo"
              /></a>
            </div>
          </div>
          <div class="bottom">
            Lorem ipsum dolor sit, amet consectetur adipisicing elit. Quisquam,
            dolorum! In, ad, deserunt cupiditate repellat explicabo
            maiorerepellat explicabo maiore
          </div>
        </div>
        <div class="keen-slider__slide number-slide1">
          <div class="top__icon">
            <a href="#"
              ><img src="../../../assets/icon/facebook.png" alt="logo"
            /></a>
            <div class="share">
              <a href="#"
                ><img src="../../../assets/icon/share-black.png" alt="logo"
              /></a>
            </div>
          </div>
          <div class="bottom">
            Lorem ipsum dolor sit, amet consectetur adipisicing elit. Quisquam,
            dolorum! In, ad, deserunt cupiditate repellat explicabo
            maiorerepellat explicabo maiore
          </div>
        </div>
        <div class="keen-slider__slide number-slide1">
          <div class="top__icon">
            <a href="#"
              ><img src="../../../assets/icon/facebook.png" alt="logo"
            /></a>
            <div class="share">
              <a href="#"
                ><img src="../../../assets/icon/share-black.png" alt="logo"
              /></a>
            </div>
          </div>
          <div class="bottom">
            Lorem ipsum dolor sit, amet consectetur adipisicing elit. Quisquam,
            dolorum! In, ad, deserunt cupiditate repellat explicabo
            maiorerepellat explicabo maiore
          </div>
        </div>
        <div class="keen-slider__slide number-slide1">
          <div class="top__icon">
            <a href="#"
              ><img src="../../../assets/icon/facebook.png" alt="logo"
            /></a>
            <div class="share">
              <a href="#"
                ><img src="../../../assets/icon/share-black.png" alt="logo"
              /></a>
            </div>
          </div>
          <div class="bottom">
            Lorem ipsum dolor sit, amet consectetur adipisicing elit. Quisquam,
            dolorum! In, ad, deserunt cupiditate repellat explicabo
            maiorerepellat explicabo maiore
          </div>
        </div>
        <div class="keen-slider__slide number-slide1">
          <div class="top__icon">
            <a href="#"
              ><img src="../../../assets/icon/facebook.png" alt="logo"
            /></a>
            <div class="share">
              <a href="#"
                ><img src="../../../assets/icon/share-black.png" alt="logo"
              /></a>
            </div>
          </div>
          <div class="bottom">
            Lorem ipsum dolor sit, amet consectetur adipisicing elit. Quisquam,
            dolorum! In, ad, deserunt cupiditate repellat explicabo
            maiorerepellat explicabo maiore
          </div>
        </div>
        <div class="keen-slider__slide number-slide1">
          <div class="top__icon">
            <a href="#"
              ><img src="../../../assets/icon/facebook.png" alt="logo"
            /></a>
            <div class="share">
              <a href="#"
                ><img src="../../../assets/icon/share-black.png" alt="logo"
              /></a>
            </div>
          </div>
          <div class="bottom">
            Lorem ipsum dolor sit, amet consectetur adipisicing elit. Quisquam,
            dolorum! In, ad, deserunt cupiditate repellat explicabo
            maiorerepellat explicabo maiore
          </div>
        </div>
        <div class="keen-slider__slide number-slide1">
          <div class="top__icon">
            <a href="#"
              ><img src="../../../assets/icon/facebook.png" alt="logo"
            /></a>
            <div class="share">
              <a href="#"
                ><img src="../../../assets/icon/share-black.png" alt="logo"
              /></a>
            </div>
          </div>
          <div class="bottom">
            Lorem ipsum dolor sit, amet consectetur adipisicing elit. Quisquam,
            dolorum! In, ad, deserunt cupiditate repellat explicabo
            maiorerepellat explicabo maiore
          </div>
        </div>
        <div class="keen-slider__slide number-slide1">
          <div class="top__icon">
            <a href="#"
              ><img src="../../../assets/icon/facebook.png" alt="logo"
            /></a>
            <div class="share">
              <a href="#"
                ><img src="../../../assets/icon/share-black.png" alt="logo"
              /></a>
            </div>
          </div>
          <div class="bottom">
            Lorem ipsum dolor sit, amet consectetur adipisicing elit. Quisquam,
            dolorum! In, ad, deserunt cupiditate repellat explicabo
            maiorerepellat explicabo maiore
          </div>
        </div>
      </div>
    </div>
    <div class="arrow__center">
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
          d="M15 8a.5.5 0 0 0-.5-.5H2.707l3.147-3.146a.5.5 0 1 0-.708-.708l-4 4a.5.5 0 0 0 0 .708l4 4a.5.5 0 0 0 .708-.708L2.707 8.5H14.5A.5.5 0 0 0 15 8z"
        />
      </svg>
      <span class="count"
        ><b>0{{ this.current }}</b
        >/10</span
      >
      <svg
        v-if="slider"
        @click="slider.next()"
        :class="{
          arrow: true,
          'arrow--right': true,
          'arrow--disabled': current === slider.details().size - 1,
        }"
        xmlns="http://www.w3.org/2000/svg"
        viewBox="0 0 24 24"
      >
        <path
          d="M1 8a.5.5 0 0 1 .5-.5h11.793l-3.147-3.146a.5.5 0 0 1 .708-.708l4 4a.5.5 0 0 1 0 .708l-4 4a.5.5 0 0 1-.708-.708L13.293 8.5H1.5A.5.5 0 0 1 1 8z"
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
      return this.slider ? [...Array(this.slider.details().size).keys()] : [];
    },
  },
  data() {
    return {
      current: 1,
      slider: null,
    };
  },
  methods: {
    setPause(active) {
      this.pause = active;
      this.setInterval();
    },
    resetInterval() {
      clearInterval(this.interval);
    },
    setInterval() {
      this.resetInterval();
      this.interval = setInterval(() => {
        if (!this.pause) {
          this.slider.next();
        }
      }, 2000);
    },
  },
  mounted() {
    this.slider = new KeenSlider(this.$refs.slider, {
      loop: true,
      duration: 3000,
      dragStart: () => {
        this.setPause(true);
      },
      dragEnd: () => {
        this.setPause(false);
      },
    });
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
  font-weight: 500;
}
.number-slide1 {
  height: 350px;
  margin: 0 1rem;
  width: 330px;
  background-color: #d5ecff;
  background-image: url(../../../assets/icon/icon-background-carousel.png);
  background-repeat: no-repeat;
  background-position: 50%;
  display: flex;
  border-radius: 5px;
  flex-direction: column;
  border: 1px solid #2699fb;
  color: #2699fb;
  justify-content: space-between;
}
.top__icon {
  display: flex;
  justify-content: space-between;
  margin: 0 1rem;
  margin-top: 1rem;
}
.share {
  width: 35px;
  height: 35px;
  display: flex;
  background-color: #fff;
  justify-content: center;
  align-items: center;
  border-radius: 50%;
}
.bottom {
  margin: 0 1rem;
  margin-bottom: 1rem;
  font-size: 70%;
  text-align: justify;
  font-weight: 400;
}
.arrow__center {
  display: flex;
  justify-content: center;
  align-items: center;
  margin-top: 2rem;
}
.navigation-wrapper {
  position: relative;
}

.arrow {
  width: 50px;
  height: 50px;
  fill: #2699fb;
  cursor: pointer;
}

.arrow--left {
  right: 0;
  color: #2699fb;
  margin-top: 1rem;
}

.arrow--right {
  left: 0;
  color: #2699fb;
  margin-top: 1rem;
}

.arrow--disabled {
  fill: #d5ecff;
}
.count {
  font-size: 20px;
  font-weight: 500;
  color: #2699fb;
  margin: 0 1rem;
}
</style>



