<template>
  <div id="app" :class="showDarkTheme ? 'dark-theme' : ''">
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
#component-container {
  padding: 15px 1rem;
  max-width: 600px;
  margin: 0 auto;
  padding: 0rem 0rem 4rem 0rem;
}
</style>
