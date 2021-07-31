<template>
  <div class="main">
    <div class="top">
      <div class="title">GAME COMMUNITY HUB</div>
      <div class="title__child">Live Game Updates</div>
      <Slide />
      <div class="row poster">
        <div class="col-3 title__post">All Posts</div>
        <div class="col-6">
          <div class="icon">
            <a href="#"
              ><img src="../../assets/icon/twitter-circle.png" alt="icon"
            /></a>
            <a href="#"
              ><img src="../../assets/icon/instagram.png" alt="icon"
            /></a>
            <a href="#"
              ><img src="../../assets/icon/facebook-icon.png" alt="icon"
            /></a>
          </div>
        </div>
        <div class="col-3">
          <input class="search__input" type="text" placeholder="Search" />
        </div>
      </div>
    </div>
    <SlidePost />
  </div>
</template>
<script>
import Slide from "./Slide.vue";
import SlidePost from "./SlidePost.vue";
export default {
  components: {
    Slide,
    SlidePost,
  },
};
</script>

<style scoped>
.main {
  height: 100vh;
  padding: 65px 0;
}
.top {
  padding: 0 528px;
}
.title,
.title__child {
  font-size: 35px;
  color: #2699fb;
  font-weight: 700;
}
.title__child {
  font-size: 15px;
  margin-bottom: 1rem;
}
.poster {
  margin: 1rem 0;
  margin-bottom: 3rem;
  margin-top: 3rem;
}
.row > * {
  padding-left: 0;
  padding-right: 0;
}
.title__post {
  font-size: 20px;
  font-weight: 700;
  color: #2699fb;
}
.col-6 {
  display: flex;
  justify-content: flex-end;
}
.icon img {
  width: 35px;
  margin: 0 0.5rem;
  height: 35px;
}
.search__input {
  width: 100%;
  padding: 8px 14px;
  background-color: transparent;
  transition: transform 250ms ease-in-out;
  font-size: 15px;
  line-height: 16px;
  color: #2699fb;
  background-color: transparent;
  background-image: url(../../assets/icon/Search.png);
  background-repeat: no-repeat;
  background-size: 18px 18px;
  background-position: 95% center;
  border-radius: 3px;
  border: 1px solid #2699fb;
  transition: all 250ms ease-in-out;
  backface-visibility: hidden;
  transform-style: preserve-3d;
}
.search__input::placeholder {
  color: #2699fb;
}
.search__input:hover,
.search__input:focus,
.search__input:active {
  border: 1px solid #2699fb;
}
</style>