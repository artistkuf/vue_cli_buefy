<template>
  <b-carousel>
    <b-carousel-item v-for="(carousel, i) in carousels" :key="i">
      <section :class="`hero is-medium main__carousel is-${carousel.color}`">
        <h1 class="title">{{ carousel.text }}</h1>
        <img :src="carousel.image" :alt="carousel.text" />
      </section>
    </b-carousel-item>
  </b-carousel>
</template>

<script>
export default {
  name: "MainCarousel",
  data() {
    return {
      carousels: [
        {
          text: "Slide 1",
          color: "primary",
          image: "https://picsum.photos/id/0/1230/500",
        },
        {
          text: "Slide 2",
          color: "info",
          image: "https://picsum.photos/id/0/1230/500",
        },
        {
          text: "Slide 3",
          color: "success",
          image: "https://picsum.photos/id/0/1230/500",
        },
        {
          text: "Slide 4",
          color: "success",
          image: "https://picsum.photos/id/0/1230/500",
        },
        {
          text: "Slide 5",
          color: "danger",
          image: "https://picsum.photos/id/0/1230/500",
        },
      ],
    };
  },
};
</script>

<style lang="scss">
.main__carousel {
  position: relative;
  h1 {
    position: absolute;
    width: 100%;
    top: 30%;
  }
}
.carousel-arrow .icon {
  color: greenyellow !important;
}
</style>
