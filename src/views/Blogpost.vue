<template>
  <div>
    <h1>{{ post.title }}</h1>
    <div class="head-image"><img :src="post.headImage" /></div>
    <div v-html="post.text"></div>
    <!-- <p>{{ post.text }}</p> -->
    <div class="blog-slider">
      <div class="right-arrow" @click="selectPreviousImage()">
        <i class="fas fa-chevron-right"></i>
      </div>
      <img
        class="slider-image"
        :src="post.slideshow[selectedImage].img"
        :alt="post.slideshow[selectedImage].caption"
      />
      <div class="left-arrow" @click="selectNextImage()">
        <i class="fas fa-chevron-left"></i>
      </div>
    </div>
    <div class="caption-container">
      <caption>
        {{
          post.slideshow[selectedImage].caption
        }}
      </caption>
    </div>
  </div>
</template>

<script lang="ts">
import Vue from "vue";
import axios from "axios";

export default Vue.extend({
  data() {
    return {
      selectedImage: 0,
      post: {
        title: String,
        headImage: String,
        text: String,
        slideshow: [],
      },
    };
  },
  async mounted() {
    try {
      const id = this.$route.params.index;
      const response = await axios.get(`http://localhost:3000/posts/${id}`);
      this.post = response.data;
      console.log(this.post);
    } catch (error) {
      console.log(error);
    }
  },
  methods: {
    selectPreviousImage() {
      if (this.selectedImage == 0) {
        this.selectedImage = this.post.slideshow.length - 1;
      } else {
        this.selectedImage -= 1;
      }
    },
    selectNextImage() {
      if (this.selectedImage == this.post.slideshow.length - 1) {
        this.selectedImage = 0;
      } else {
        this.selectedImage += 1;
      }
    },
  },
});
</script>

<style scoped lang = "scss">
@import "../../styles/blogpost.scss";
</style>