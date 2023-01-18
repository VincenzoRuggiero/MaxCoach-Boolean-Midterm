<script>
import CTAbutton from "../CTAbutton.vue";

export default {
  name: "CoursesCards",
  components: {
    CTAbutton,
  },
};
</script>

<template>
  <div class="card" v-for="n in 6">
    <img
      class="img-fluid"
      src="../../assets/styles/images/motivation-course-06-480x298.jpg"
      alt="" />
    <div class="card-content p-4">
      <h5 class="card-price"><span class="big-price">$30</span>.00</h5>
      <h6>How to be Succesful: Create A Growth Mindset For Success</h6>
      <span>3 Lessons</span> <span>50 Students</span>
    </div>
  </div>
</template>

<style lang="scss"></style>
