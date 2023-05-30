<script>
export default {
  name: "ArticleCard",
  props: ["image", "date", "title", "excerpt"],
};
</script>

<template>
  <div class="article-card col-6 col-lg-3">
    <img class="img-fluid" :src="image" alt="Article featured image" />
    <span class="grey"
      ><font-awesome-icon class="icon" icon="fa-regular fa-calendar" />
      {{ date }}</span
    >
    <h6>{{ title }}</h6>
    <p class="grey">{{ excerpt }}</p>
  </div>
</template>

<style lang="scss">
.article-card {
  padding: 0.5rem;

  img:hover {
    transform: scale3d(1.1, 1.1, 1.1);
    transition: all 1.5s cubic-bezier(0, 0, 0, 1);
  }

  span {
    display: inline-block;
    margin-top: 1.3rem;
    font-size: 0.9rem;

    .icon {
      margin-right: 0.3rem;
    }
  }

  h6 {
    font-size: 1.3rem;
    line-height: 2rem;
    padding: 1rem 0;
  }
}
</style>
