<template>
  <div>
    <NavbarDesktop @darktheme="$emit('darktheme', $event)" />
    <NavbarMobile @darktheme="$emit('darktheme', $event)" />
  </div>
</template>

<script lang="ts">
import Vue from "vue";
import NavbarDesktop from "@/components/Navbars/NavbarDesktop.vue";
import NavbarMobile from "@/components/Navbars/NavbarMobile.vue";

export default Vue.extend({
  components: {
    NavbarDesktop,
    NavbarMobile,
  },
});
</script>

<style scoped lang="scss">
</style>