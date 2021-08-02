<template>
  <div class="section">
    <Hotposter class="section__item" />
    <Register class="section__item" />
    <GameCommunityHub class="section__item" />
    <SpecialEvent class="section__item" />
    <GameContent class="section__item" />
  </div>
</template>

<script>
import Hotposter from "../ChildMain/Child/Hotposter.vue";
import Register from "../ChildMain/Child/Register.vue";
import GameCommunityHub from "../ChildMain/Child/GameCommunityHub.vue";
import SpecialEvent from "../ChildMain/Child/SpecialEvent.vue";
import GameContent from "../ChildMain/Child/GameContent.vue";
export default {
  components: {
    Hotposter,
    Register,
    GameCommunityHub,
    SpecialEvent,
    GameContent,
  },
  mounted() {},
};
</script>

<style>
</style>