<script>
export default {
  name: "CoursesCards",
  data() {
    return {
      cardContents: [
        {
          img: "motivation-course-06-480x298.jpg",
          price: 30,
          cents: "00",
          title: "How to be Succesful: Create A Growth Mindset For Success",
          lessons: 3,
        },
        {
          img: "motivation-course-05-480x298.jpg",
          price: 30,
          cents: "00",
          title: "How to Build Confidence in Your Abilities",
          lessons: 1,
        },
        {
          img: "motivation-course-04-480x298.jpg",
          price: 20,
          cents: "00",
          title: "Productivity Machine - Focus in a Distracted World",
          lessons: 5,
        },
        {
          img: "motivation-course-03-480x298.jpg",
          price: 20,
          cents: "00",
          title: "Effective Time Management Mastery - Complete Guide",
          lessons: 18,
        },
        {
          img: "motivation-course-02-480x298.jpg",
          price: 25,
          cents: 99,
          title: "How to Build Confidence in Your Abilities",
          lessons: 1,
        },
        {
          img: "motivation-course-01-480x298.jpg",
          price: 19,
          cents: 99,
          title: "Body Language Secrets for Entrepreneurs",
          lessons: 19,
        },
      ],
    };
  },
  methods: {
    getImagePath(image) {
      return new URL(`../../assets/styles/images/${image}`, import.meta.url)
        .href;
    },
  },
};
</script>

<template>
  <div class="course-card col-4" v-for="content in cardContents">
    <img class="img-fluid" :src="getImagePath(content.img)" alt="" />
    <div class="card-content p-4">
      <h5 class="card-price green">
        <span class="big-price">${{ content.price }}</span
        >.{{ content.cents }}
      </h5>
      <h5 class="py-3 text-start course-title">
        {{ content.title }}
      </h5>
      <div class="course-info grey">
        <span
          ><font-awesome-icon class="icon" icon="fa-regular fa-file-lines" />
          {{ content.lessons }} lessons</span
        >
        <span
          ><font-awesome-icon class="icon" icon="fa-regular fa-user" /> 50
          Students</span
        >
      </div>
    </div>
  </div>
</template>

<style lang="scss" scoped>
@use "../../assets/styles/partials/variables" as *;

.course-card {
  border: none;
  padding: 0 1rem;

  .course-title {
    color: $congress-blue;
  }

  .card-price {
    font-size: 0.9rem;

    .big-price {
      font-size: 1.6rem;
    }
  }
  .course-info span {
    padding: 0 1rem;

    .icon {
      margin-right: 0.3rem;
    }
  }
}
</style>
