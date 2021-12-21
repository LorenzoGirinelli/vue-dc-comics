<template>
  <div id="app">
    <Header />,
    <Main />,
    <Icons />
  </div>
</template>

<script>
import Header from "./components/Header.vue";
import Main from "./components/Main.vue";
import Icons from "./components/Icons.vue";

export default {
  name: "App",
  components: {
    Header,
    Main,
    Icons,
  },
};
</script>

<style lang="scss">
@import './style/general.scss';
@import './style/common.scss';
</style>
