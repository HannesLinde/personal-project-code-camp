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
    <button
      @click="
        showDarkTheme = !showDarkTheme;
        say(showDarkTheme);
      "
    >
      <i class="far fa-moon"></i>
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
  },
});
</script>

<style scoped lang="scss">
@media (min-width: 401px) {
  .navbar-mobile {
    display: none;
  }
}
@media (max-width: 400px) {
  .navbar-mobile {
    text-decoration: underline #92006c;
    padding: 0.5rem;
    display: flex;
    justify-content: space-between;
    button {
      height: 1rem;
      width: 2rem;
      background-color: #92006c;
      color: #f9f871;
      border: none;
      z-index: 0;
    }
    .mobile-menu-list {
      background-color: #92006c;
      a {
        color: #f9f871;
      }
      list-style-type: none;
      display: flex;
      flex-direction: column;
      justify-content: center;
      .routes {
        width: 100vw;
        flex-direction: column;
        z-index: 1;
        li {
          padding: 0px 2px;
          &:hover {
            background-color: #f9f871;
            a {
              color: #92006c;
            }
          }
        }
      }
      .hamburger {
        display: block;
      }
    }
  }
}
</style>