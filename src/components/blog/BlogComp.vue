<script>
import ArticleCard from "./ArticleCard.vue";

export default {
  name: "BlogComp",
  components: {
    ArticleCard,
  },
  data() {
    return {
      articles: [
        {
          img: "motivation-blog-04-480x325.jpg",
          date: "May 13, 2020",
          title: "How to Stay True to Your Personal Brand",
          excerpt: "When it comes to your business or career, you want ...",
        },
        {
          img: "motivation-blog-03-480x325.jpg",
          date: "May 13, 2020",
          title: "5 Vital Lessons in 5 Years of Freelancing",
          excerpt:
            "Being self-employed and working from home, it's easy to get ...",
        },
        {
          img: "motivation-blog-02-480x325.jpg",
          date: "May 13, 2020",
          title: "11 Super Useful Tips for Small-Business Owners",
          excerpt:
            "Being a small-business owner poses a ton of challenges. We ...",
        },
        {
          img: "motivation-blog-01-480x325.jpg",
          date: "May 13, 2020",
          title: "How to Give Yourself Grace to Start Again",
          excerpt:
            "Forgive yourself for bad habits you may have started or ...",
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
  <div class="container mt-5 py-5">
    <div class="row">
      <div class="col-12">
        <span class="section-name">Blog Updated</span>
        <h2 class="py-3">
          Interesting <span class="green"> articles updated</span> daily
        </h2>
        <div class="col-12 d-flex mt-5">
          <ArticleCard
            v-for="article in articles"
            :image="getImagePath(article.img)"
            :date="article.date"
            :title="article.title"
            :excerpt="article.excerpt" />
        </div>
        <div class="col-12">
          <div class="row text-center mt-5">
            <a class="section-name green" href="#">View all posts</a>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<style lang="scss" scoped>
@use "../../assets/styles/partials/variables" as *;

.section-name {
  font-weight: bold;

  &:hover {
    color: $congress-blue;
    transition: all 0.2s ease;
  }
}
</style>
