<template>
  <div class="navbar-mobile">
    <div class="mobile-menu-list">
      <ul class="routes">
        <button id="hamburger">
          <i
            v-if="showMobile == false"
            @click="showMobile = true"
            class="fas fa-bars"
          />
          <i v-else @click="showMobile = false" class="fas fa-window-close"></i>
        </button>
        <a v-if="showMobile" href="/"><li>About</li></a>
        <a v-if="showMobile" href="/blog"><li>Blog</li></a>
        <a v-if="showMobile" href="/portfolio"><li>Portfolio</li></a>
      </ul>
    </div>
    <button @click="toggleDarkTheme()">
      <span v-if="showDarkTheme == false">🌙</span>
      <span v-if="showDarkTheme">☀️</span>
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