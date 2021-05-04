<template>
  <div
    style="
      background: linear-gradient(315deg, #92006c, #d2245a 50%, #ffb448);
      max-height: 100vh;
      overflow-y: auto;
    "
  >
    <div
      :class="showDarkTheme ? 'dark-theme' : ''"
      style="
        display: flex;
        flex-direction: column;
        min-height: 100vh;
        justify-content: space-between;
      "
    >
      <div id="app">
        <Navbar @darktheme="showDarkTheme = $event" />
        <div id="component-container">
          <router-view />
        </div>
      </div>
      <Footer />
    </div>
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
