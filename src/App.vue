<template>
  <div id="app">
    <div id="background"></div>
    <Navbar />
    <div id="component-container">
      <router-view />
    </div>
  </div>
</template>
<script lang="ts">
import Vue from "vue";
import Navbar from "@/components/Navbar.vue";
// import About from "@/components/About.vue";
export default Vue.extend({
  components: {
    Navbar,
    // About,
  },
});
</script>
<style lang="scss">
@import "../styles/index.scss";
</style>
