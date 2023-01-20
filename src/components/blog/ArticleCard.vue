<script>
export default {
  name: "ArticleCard",
  props: ["image", "date", "title", "excerpt"],
};
</script>

<template>
  <div class="article-card">
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
  width: calc(100% / 4 - 1rem);
  padding: 0.5rem;

  img:hover {
    transform: scale(1.1);
    transition: all 0.2s ease-in;
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
