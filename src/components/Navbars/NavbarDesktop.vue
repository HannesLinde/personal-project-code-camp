<template>
  <div class="navbar-desktop">
    <ul class="routes">
      <li><router-link to="/">About</router-link></li>
      <li><router-link to="/blog">Blog</router-link></li>
      <li><router-link to="/portfolio">Portfolio</router-link></li>
    </ul>
    <button @click="toggleDarkTheme()">
      <i v-if="showDarkTheme == false" class="far fa-moon"></i>
      <i v-if="showDarkTheme" class="fas fa-rainbow"></i>
    </button>
  </div>
</template>

<script lang="ts">
import Vue from "vue";

export default Vue.extend({
  methods: {
    say(stuff: string | boolean) {
      console.log(stuff);
    },
    toggleDarkTheme() {
      this.showDarkTheme = !this.showDarkTheme;
      this.$emit("darktheme", this.showDarkTheme);
    },
  },
  data() {
    return {
      showDarkTheme: false,
    };
  },
});
</script>

<style scoped lang="scss">
</style>