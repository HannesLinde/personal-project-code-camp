<template>
  <div id="app" :class="showDarkTheme ? 'dark-theme' : ''">
    <div class="background"></div>
    <Navbar @darktheme="showDarkTheme = $event" />

    <div id="component-container">
      <router-view />
    </div>
    <Footer />
  </div>
</template>
<script lang="ts">
import Vue from "vue";
import Navbar from "@/components/Navbar.vue";
import Footer from "@/components/Footer.vue";

export default Vue.extend({
  data() {
    return {
      showDarkTheme: false,
    };
  },
  methods: {
    say(stuff: string | boolean) {
      console.log(stuff);
    },
  },
  components: {
    Navbar,
    Footer,
  },
});
</script>
<style lang="scss">
@import "../styles/index.scss";
</style>
