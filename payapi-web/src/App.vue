<template>
  <div id="app">
    <navBar />
    <router-view />
    <footerBar />
  </div>
</template>

<style>
#app {
  height: 100%;
  text-align: center;
  color: #2c3e50;
}
</style>

<script>
import navBar from "./components/NavigationBar.vue";
import footerBar from "./components/FooterBar.vue";

export default {
  components: {
    navBar,
    footerBar,
  },
};
</script>