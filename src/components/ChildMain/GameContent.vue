<template>
  <div class="main">
    <div class="title">Exclusive Game Content</div>
    <div class="title__child">
      Lorem ipsum, dolor sit amet consectetur adipisicing elit. Provident
      aliquid quisquam doloremque modi sapiente! Ex obcaecati soluta assumenda
      ratione ad fugiat enim autem aliquid,
    </div>
    <SliderContent />
  </div>
</template>

<script>
import SliderContent from "./SliderContent.vue";
export default {
  components: {
    SliderContent,
  },
};
</script>

<style scoped>
.main {
  background-color: #fff;
  height: 100vh;
  padding: 200px 0;
  padding-bottom: 80px;
}
.title {
  text-transform: uppercase;
}
.title,
.title__child {
  padding-left: 528px;
  padding-right: 528px;
  font-size: 35px;
  color: #2699fb;
  font-weight: 700;
}
.title__child {
  font-size: 15px;
  font-weight: 300;
  margin-bottom: 5rem;
}
</style>