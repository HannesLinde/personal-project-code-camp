<template>
  <div class="footer">
    <span>
      Thanks for visiting. Feel free to
      <a href="mailto:hanneslinde@posteo.de">contact me for web dev jobs</a>.
      &#x1F496; &#x1F496; &#x1F496;
    </span>
  </div>
</template>

<script lang="ts">
import Vue from "vue";

export default Vue.extend({});
</script>

<style scoped lang="scss">
.footer {
  padding: 5px 0px;
  position: absolute;
  bottom: 0px;
  width: 100vw;
  background-color: #92006c;
  color: #d3cec4;
  display: flex;
  justify-content: center;

  a {
    color: #d3cec4;
    text-decoration: underline #d3cec4;
  }

  span {
    max-width: 600px;
    text-align: center;
  }
}
</style>