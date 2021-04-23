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
import arizonaUni from "../assets/img/arizonauni.png";
import clearchannel from "../assets/img/clearchannel.png";
import designit from "../assets/img/designit.png";
import uniflorida from "../assets/img/uniflorida.png";
import topps from "../assets/img/topps.png";

export const posts = [
  {
    title: "my first blog entry",
    headImage: arizonaUni,
    text: `Lorem ipsum dolor, sit amet consectetur adipisicing elit. Esse inventore praesentium laudantium voluptatibus ipsa provident impedit saepe eaque. Et temporibus sequi accusamus nemo non minima debitis minus laudantium iste unde.
  Voluptatem, deserunt. Quisquam quas blanditiis pariatur iusto laudantium perspiciatis, ab incidunt ipsam veniam excepturi quibusdam modi distinctio saepe eius, quam aperiam quaerat accusantium. Aliquid, magni dolorum voluptas praesentium repudiandae repellendus.
  Reiciendis iusto quo aspernatur harum perferendis non fuga, nesciunt, veniam assumenda, ipsam rem optio! Quisquam nobis mollitia in omnis quo, odio autem? Laboriosam quis minus ab animi cupiditate doloremque ea.`,
    slideShow: [
      { img: clearchannel, caption: "This is a logo from clearcello" },
      { img: designit, caption: "This is a logo from designit" },
      { img: uniflorida, caption: "This is a logo from University of Florida" },
      { img: topps, caption: "This is a logo of Topps" },
    ],
  },
  {
    title: "my second blog Ddventure",
    text: `Lorem ipsum dolor, sit amet consectetur adipisicing elit. Esse inventore praesentium laudantium voluptatibus ipsa provident impedit saepe eaque. Et temporibus sequi accusamus nemo non minima debitis minus laudantium iste unde.
  Voluptatem, deserunt. Quisquam quas blanditiis pariatur iusto laudantium perspiciatis, ab incidunt ipsam veniam excepturi quibusdam modi distinctio saepe eius, quam aperiam quaerat accusantium. Aliquid, magni dolorum voluptas praesentium repudiandae repellendus.
  Reiciendis iusto quo aspernatur harum perferendis non fuga, nesciunt, veniam assumenda, ipsam rem optio! Quisquam nobis mollitia in omnis quo, odio autem? Laboriosam quis minus ab animi cupiditate doloremque ea.`,
  },
  {
    title: "my thirs blog blackout",
    text: `Lorem ipsum dolor, sit amet consectetur adipisicing elit. Esse inventore praesentium laudantium voluptatibus ipsa provident impedit saepe eaque. Et temporibus sequi accusamus nemo non minima debitis minus laudantium iste unde.
  Voluptatem, deserunt. Quisquam quas blanditiis pariatur iusto laudantium perspiciatis, ab incidunt ipsam veniam excepturi quibusdam modi distinctio saepe eius, quam aperiam quaerat accusantium. Aliquid, magni dolorum voluptas praesentium repudiandae repellendus.
  Reiciendis iusto quo aspernatur harum perferendis non fuga, nesciunt, veniam assumenda, ipsam rem optio! Quisquam nobis mollitia in omnis quo, odio autem? Laboriosam quis minus ab animi cupiditate doloremque ea.`,
  },
];

export default Vue.extend({
  data() {
    return {
      posts,
    };
  },
});
</script>

<style scoped>
</style>