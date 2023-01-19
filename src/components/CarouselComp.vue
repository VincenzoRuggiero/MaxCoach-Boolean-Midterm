<script>
import CarouselCard from "./CarouselCard.vue";

export default {
  name: "CarouselComp",
  components: {
    CarouselCard,
  },
  data() {
    return {
      testimonials: [
        {
          comment:
            "I am free to learn at my own pace, follow my own schedule and choose the subject I want to learn from the syllabus. Great study portal for people like me.",
          img: "testimonial-avata-02.jpg",
          name: "Mina Hollace",
          job: "/Freelancer",
        },
      ],
    };
  },
  methods: {
    getImagePath(image) {
      return new URL(`../assets/styles/images/${image}`, import.meta.url).href;
    },
  },
};
</script>

<template>
  <div v-for="testimonial in testimonials">
    <CarouselCard
      :review="testimonial.comment"
      :userPic="getImagePath(testimonial.img)"
      :userName="testimonial.name"
      :userJob="testimonial.job" />
  </div>
</template>

<style lang=""></style>
