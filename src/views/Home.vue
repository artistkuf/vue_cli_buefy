<template>
  <div>
    <MainCarousel id="home" />
    <MainComp id="anchor" />
  </div>
</template>

<script>
import MainCarousel from "@/components/MainCarousel.vue";
import MainComp from "@/components/MainComp.vue";

export default {
  components: {
    MainCarousel,
    MainComp,
  },
};
</script>

<style></style>
