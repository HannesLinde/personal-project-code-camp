<template>
  <div>
    <h1>{{ post.title }}</h1>
    <img :src="post.headImage" />
    <p>{{ post.text }}</p>
    <div class="blog-slider">
      <img src="" />
      <caption></caption>
    </div>
  </div>
</template>

<script lang="ts">
import Vue from "vue";
import { posts } from "@/views/Blog.vue";

export default Vue.extend({
  computed: {
    post() {
      return posts[Number(this.$route.params.index)];
    },
  },
});
</script>

<style scoped>
</style>