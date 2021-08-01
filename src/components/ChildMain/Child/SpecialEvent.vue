<template>
  <div class="main">
    <div class="title">Special Events & Promotional</div>
    <div class="title__child">
      Lorem ipsum, dolor sit amet consectetur adipisicing elit. Provident
      aliquid quisquam doloremque modi sapiente! Ex obcaecati soluta assumenda
      ratione ad fugiat enim autem aliquid,
    </div>
    <SliderEvent />
  </div>
</template>

<script>
import SliderEvent from "../Slider/SliderEvent.vue";
export default {
  components: {
    SliderEvent,
  },
};
</script>

<style scoped>
.main {
  background-color: #d8edff;
  height: 100vh;
  padding: 80px 0;
}
.title {
  text-transform: uppercase;
}
.title,
.title__child {
  padding-left: 328px;
  padding-right: 200px;
  font-size: 35px;
  color: #2699fb;
  font-weight: 700;
}
.title__child {
  font-size: 15px;
  font-weight: 300;
  margin-bottom: 1rem;
}

@media only screen and (max-width: 430px) {
  .main {
    padding: 20px 20px;
  }
  .title,
  .title__child {
    padding-left: 0;
    padding-right: 0;
    font-size: 20px;
    width: 50%;
    text-transform: capitalize;
  }
  .title__child {
    font-size: 15px;
    width: 100%;
    height: 60px;
    -webkit-box-orient: vertical;
    overflow: hidden;
    display: -webkit-box;
  }
}
</style>