<script>
export default {
  name: "CarouselCard",
  props: ["review", "userPic", "userName", "userJob"],
};
</script>

<template>
  <div class="review-card">
    <p class="comment">{{ review }}</p>
    <img :src="userPic" alt="User Profile Image" />
    <h3>{{ userName }}</h3>
    <p class="grey">{{ userJob }}</p>
  </div>
</template>

<style lang="scss" scoped>
.review-card {
  padding: 5rem;

  .comment {
    font-size: 2.5rem;
    padding: 0 7rem;
  }

  img {
    width: 10%;
    border-radius: 50%;
    margin: 2rem 0;
  }

  h3 {
    margin-bottom: 2rem;
  }
}
</style>
