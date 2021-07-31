<template>
  <div id="app">
    <Header />
    <Hotposter />
    <Register />
    <GameCommunityHub />
    <SpecialEvent />
    <Footer />
  </div>
</template>

<script>
import Header from "./components/Header.vue";
import Hotposter from "./components/ChildMain/Hotposter.vue";
import Register from "./components/ChildMain/Register.vue";
import GameCommunityHub from "./components/ChildMain/GameCommunityHub.vue";
import SpecialEvent from "./components/ChildMain/SpecialEvent.vue";
import Footer from "./components/Footer.vue";
export default {
  name: "App",
  components: {
    Header,
    Hotposter,
    Register,
    GameCommunityHub,
    SpecialEvent,
    Footer,
  },
};
</script>

<style>
@import "./assets/css/style.css";
</style>
