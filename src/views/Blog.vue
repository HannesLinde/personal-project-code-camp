<template>
  <div>
    <h1>Here comes the blog</h1>
    <div v-for="(post, index) in posts" :key="post.title">
      <router-link :to="`/blog/${index}`">{{ post.title }}</router-link>
    </div>
  </div>
</template>

<script lang="ts">
import Vue from "vue";
import axios from "axios";

export default Vue.extend({
  data() {
    return {
      posts: [],
    };
  },
  async mounted() {
    try {
      const blogPosts = await axios.get("http://localhost:3000/posts");
      this.posts = blogPosts.data;
    } catch (error) {
      console.log(error);
    }
  },
});
</script>

<style scoped lang="scss">
@import "../../styles/blog.scss";
@import "../../styles/blogpost.scss";
</style>