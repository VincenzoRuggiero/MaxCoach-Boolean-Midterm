<script>
import HeaderComp from "./components/HeaderComp.vue";
import ResultsComp from "./components/simpleComps/ResultsComp.vue";
import PresentationComp from "./components/PresentationComp.vue";
import CoursesShop from "./components/shop/CoursesShop.vue";
import CourseCards from "./components/shop/CoursesCards.vue";
import BooksShop from "./components/shop/BooksShop.vue";
import ClientsComp from "./components/simpleComps/ClientsComp.vue";
import TestimonialsComp from "./components/TestimonialsComp.vue";
import BlogComp from "./components/blog/BlogComp.vue";
import FooterComp from "./components/FooterComp.vue";

export default {
  components: {
    HeaderComp,
    ResultsComp,
    PresentationComp,
    CoursesShop,
    CourseCards,
    BooksShop,
    ClientsComp,
    TestimonialsComp,
    BlogComp,
    FooterComp,
  },
};
</script>

<template>
  <HeaderComp />
  <ResultsComp />
  <PresentationComp />
  <CoursesShop />
  <BooksShop />
  <ClientsComp />
  <TestimonialsComp />
  <BlogComp />
  <FooterComp />
</template>

<style lang="scss">
@use "../node_modules/bootstrap/scss/bootstrap.scss" as *;
@use "./assets/styles/general.scss" as *;
@use "./assets/styles/partials/variables" as *;

.section-name {
  text-transform: uppercase;
  letter-spacing: 3px;
  font-size: 1.2rem;
}

.green {
  color: $mountain-meadow;
}

.grey {
  color: $corduray;
}
</style>
