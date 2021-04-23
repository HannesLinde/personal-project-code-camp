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
        :src="post.slideShow[selectedImage].img"
        :alt="post.slideShow[selectedImage].caption"
      />
      <div class="left-arrow" @click="selectNextImage()">
        <i class="fas fa-chevron-left"></i>
      </div>
    </div>
    <div class="caption-container">
      <caption>
        {{
          post.slideShow[selectedImage].caption
        }}
      </caption>
    </div>
  </div>
</template>

<script lang="ts">
import Vue from "vue";
import { posts as untypedposts } from "@/views/Blog.vue";
const posts = untypedposts as any;

export default Vue.extend({
  data() {
    return {
      selectedImage: 0,
    };
  },
  computed: {
    post() {
      return posts[Number(this.$route.params.index)];
    },
  },
  methods: {
    selectPreviousImage() {
      if (this.selectedImage == 0) {
        this.selectedImage =
          posts[Number(this.$route.params.index)].slideShow.length - 1;
      } else {
        this.selectedImage -= 1;
      }
    },
    selectNextImage() {
      if (
        this.selectedImage ==
        posts[Number(this.$route.params.index)].slideShow.length - 1
      ) {
        this.selectedImage = 0;
      } else {
        this.selectedImage += 1;
      }
    },
  },
});
</script>

<style scoped lang = "scss">
.head-image {
  padding: 10px 0px;
  display: flex;
  justify-content: center;
}
.blog-slider {
  margin-top: 1rem;
  padding: 5px;
  background-color: #121212;
  position: relative;
  display: flex;
  justify-items: center;
  align-items: center;
}

.right-arrow {
  color: white;
  position: absolute;
  right: 0px;
  cursor: pointer;
}

.left-arrow {
  color: white;
  position: absolute;
  left: 0px;
  cursor: pointer;
}

.slider-image {
  margin: 0 auto;
}

.caption-container {
  display: flex;
  justify-content: center;
}
caption {
  font-size: 14px;
  color: #ddd;
  width: 300px;
  text-align: center;
}

blockquote {
  font-style: italic;
  font-size: 24px;
}
</style>