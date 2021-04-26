<template>
  <div class="navbar-mobile">
    <div class="mobile-menu-list">
      <button class="hamburger">
        <i
          v-if="showMobile == false"
          @click="showMobile = true"
          class="fas fa-bars"
        />
        <i v-else @click="showMobile = false" class="fas fa-window-close"></i>
      </button>
      <ul v-if="showMobile" class="routes">
        <li><a href="/">About</a></li>
        <li><a href="/blog">Blog</a></li>
        <li><a href="/portfolio">Portfolio</a></li>
      </ul>
    </div>
    <button @click="toggleDarkTheme()">
      <i v-if="showDarkTheme == false" class="far fa-moon"></i>
      <i v-if="showDarkTheme" class="fas fa-rainbow"></i>
    </button>
  </div>
</template>

<script lang="ts">
import Vue from "vue";

export default Vue.extend({
  data() {
    return {
      showMobile: false,
      showDarkTheme: false,
    };
  },
  methods: {
    say(stuff: any) {
      console.log(stuff);
    },
    toggleDarkTheme() {
      this.showDarkTheme = !this.showDarkTheme;
      this.$emit("darktheme", this.showDarkTheme);
    },
  },
});
</script>

<style scoped lang="scss">
</style>