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
@media (max-width: 400px) {
  .navbar-desktop {
    display: none;
  }
}
@media (min-width: 401px) {
  .navbar-desktop {
    text-decoration: overline #92006c;
    margin: 0 auto;
    padding: 2rem 0rem;
    max-width: 600px;
    display: flex;
    justify-content: space-between;
    align-items: center;
    .routes {
      list-style-type: none;
      display: flex;
      justify-content: space-evenly;
      li {
        padding: 10px 15px;
        padding-left: 0px;
        &:hover {
          background-color: #92006c;
          a {
            color: #f9f871;
          }
        }
      }
    }
    button {
      height: 1rem;
      width: 2rem;
      background-color: #92006c;
      color: #f9f871;
      border: none;
      z-index: 0;
      cursor: pointer;
    }
  }
}
</style>