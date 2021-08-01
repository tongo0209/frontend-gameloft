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
  padding-left: 328px;
  padding-right: 150px;
  font-size: 35px;
  color: #2699fb;
  font-weight: 700;
}
.title__child {
  font-size: 15px;
  font-weight: 300;
  margin-bottom: 3rem;
}

@media only screen and (max-width: 430px) {
  .main {
    height: 60vh;
    padding: 30px 0;
  }
  .title {
    text-transform: capitalize;
  }
  .title,
  .title__child {
    padding-left: 20px;
    padding-right: 20px;
    font-size: 20px;
    color: #2699fb;
    font-weight: 700;
  }
  .title__child {
    font-size: 15px;
    font-weight: 300;
    margin-bottom: 3rem;
    margin-top: 2rem;
    height: 60px;
    -webkit-box-orient: vertical;
    overflow: hidden;
    display: -webkit-box;
  }
}
</style>