<template>
  <div id="app">
    <div v-bind:class="{ background: showDarkTheme }"></div>
    <Navbar :showDarkTheme="false" />
    <div id="component-container">
      <router-view />
    </div>
  </div>
</template>
<script lang="ts">
import Vue from "vue";
import Navbar from "@/components/Navbar.vue";

export default Vue.extend({
  components: {
    Navbar,
  },
  data() {
    return {
      showDarkTheme: false,
    };
  },
  computed: {
    showDarktheme() {
      return this.showDarkTheme;
    },
  },
});
</script>
<style lang="scss">
@import "../styles/index.scss";
</style>
