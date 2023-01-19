<script>
import ArticleCard from "./ArticleCard.vue";

export default {
  name: "BlogComp",
  components: {
    ArticleCard,
  },
};
</script>

<template>
  <div class="container py-5">
    <div class="row">
      <div class="col-12">
        <span>Blog Updated</span>
        <h2>Interesting <span> articles updated</span> daily</h2>
        <div class="col-12 d-flex">
          <ArticleCard v-for="n in 4" />
        </div>
        <div class="col-12">
          <div class="row text-center">
            <a href="#">View all posts</a>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<style lang="scss"></style>
