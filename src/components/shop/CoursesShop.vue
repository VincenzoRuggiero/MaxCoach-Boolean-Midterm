<script>
import CoursesCards from "./CoursesCards.vue";
import CTAbutton from "../CTAbutton.vue";

export default {
  name: "CoursesShop",
  components: {
    CoursesCards,
    CTAbutton,
  },
};
</script>

<template>
  <div class="container">
    <div class="row text-center">
      <div class="col-12">
        <span>Begin Your Journey at Maxcoach</span>
      </div>
      <div class="col-12">
        <h2>Latest <span>Online Courses</span></h2>
      </div>
    </div>
    <div class="col-12 d-flex flex-wrap">
      <CoursesCards />
    </div>
    <!-- <div class="col-12"> -->
    <!-- <CTAbutton /> -->
    <!-- </div> -->
  </div>
</template>

<style lang="scss"></style>
