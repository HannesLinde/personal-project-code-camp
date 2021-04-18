<template>
  <div>
    <Header></Header>
    <Hero></Hero>
    <Trial></Trial>
  </div>
</template>

<script lang="ts">
import Vue from "vue";
import Header from "@/components/Header.vue";
import Hero from "@/components/Hero.vue";
import Trial from "@/components/Trial.vue";

export default Vue.extend({
  components: {
    Header,
    Hero,
    Trial
  }
});
</script>

<style scoped lang="scss"></style>
