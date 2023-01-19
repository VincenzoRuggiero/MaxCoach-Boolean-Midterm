<script>
export default {
  name: "ArticleCard",
  props: ["image", "date", "title", "excerpt"],
};
</script>

<template>
  <div class="article-card">
    <img class="img-fluid" :src="image" alt="Article featured image" />
    <span class="grey"> {{ date }}</span>
    <h6>{{ title }}</h6>
    <p class="grey">{{ excerpt }}</p>
  </div>
</template>

<style lang="scss">
.article-card {
  padding: 0 1rem;

  span {
    display: inline-block;
    margin-top: 1.3rem;
    font-size: 0.9rem;
  }

  h6 {
    font-size: 1.3rem;
    line-height: 2rem;
    padding: 1rem 0;
  }
}
</style>
