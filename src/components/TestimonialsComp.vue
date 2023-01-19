<script>
import CarouselComp from "./CarouselComp.vue";

export default {
  name: "TestimonialsComp",
  components: {
    CarouselComp,
  },
};
</script>

<template>
  <div class="container-fluid p-relative">
    <div
      class="controls d-flex flex-column justify-content-center align-items-center justify-content-between">
      <img src="../assets/styles/images/image.png" alt="" />
      <p>1 / 4</p>
      <img src="../assets/styles/images/image (1).png" alt="" />
    </div>
    <div class="row d-flex justify-content-center">
      <div class="col-6 carousel p-5 carousel-bg waves-pattern text-center">
        <span class="section-name green">Real stories</span>
        <CarouselComp />
      </div>
      <div class="col-6 man"></div>
    </div>
  </div>
</template>

<style lang="scss">
@use "../assets/styles/partials/variables" as *;

.p-relative {
  position: relative;
}

.carousel-bg {
  background-color: $athens-grey;
}

.waves-pattern {
  background-image: url("../assets/styles/images/background-pattern-wavify.png");
}

.man {
  background-image: url("../assets/styles/images/home-movation-testimonial-image-768x562.jpg");
  background-size: cover;
}

.controls {
  // text-align: center;
  padding: 0.9rem;
  width: 100px;
  height: 100px;
  background-color: $white;
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  z-index: 1;
  border-radius: 50%;

  p {
    margin: 0;
  }

  img {
    width: 1rem;
  }
}
</style>
