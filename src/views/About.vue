<template>
  <div>
    <div>
      <span style="white-space: pre-line"
        >Hi, I am Hannes. I am a Software Developer, focussing on frontend
        development. If you’re interested in working with me, check out my
        <a href="https://github.com/HannesLinde">Github account</a> (one day in
        future: my portfolio) and don’t hesitate to
        <a href="mailto:hanneslinde@posteo.de">contact me</a>.</span
      >
      <br />
      <br />
      If you’re interested in my views on family life, progressive politics,
      skateboarding and rugby, sit back, relax and read my
      <router-link to="/blog">blog</router-link> or
      <a href="https://twitter.com/linde_hannes">twitter</a> (or rather: the
      people I follow on twitter).
      <br />
      <br />
      To make sure I don’t send a CV to anyone anymore, the following list
      hopefully ticks all the boxes:
      <ul>
        <li>
          Relevant work experience before programming: Campaigner and founding
          staff of
          <a href="https://finanzwende.de">Finanzwende</a>
        </li>
        <li>Born 1990 in Germany</li>
        <li>Bachelor of Science in Forestry (2014, Dresden)</li>
        <li>Master of Science in Environmental Science (2017, Freiburg)</li>
        <li>Standing up for Climate Justice since 2015</li>
      </ul>
    </div>
  </div>
</template>

<script lang="ts">
import Vue from "vue";
import About from "@/components/About.vue";
export default Vue.extend({
  components: {},
});
</script>

<style scoped lang="scss">
@import "../../styles/about.scss";
</style>
