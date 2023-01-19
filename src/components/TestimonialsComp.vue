<script>
export default {
  name: "TestimonialsComp",
};
</script>

<template>
  <div class="container-fluid">
    <div class="row d-flex justify-content-center">
      <div class="col-6 carousel-bg waves-pattern"></div>
      <div class="col-6 man"></div>
    </div>
  </div>
</template>

<style lang="scss">
@use "../assets/styles/partials/variables" as *;

.carousel-bg {
  background-color: $athens-grey;
  height: 60vh;
}

.waves-pattern {
  background-image: url("../assets/styles/images/background-pattern-wavify.png");
}

.man {
  background-image: url("../assets/styles/images/home-movation-testimonial-image-768x562.jpg");
  background-repeat: no-repeat;
}
</style>
