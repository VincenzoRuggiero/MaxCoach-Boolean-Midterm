<script>
import HeaderComp from "./components/HeaderComp.vue";
import ResultsComp from "./components/ResultsComp.vue";
import PresentationComp from "./components/PresentationComp.vue";
import CoursesShop from "./components/shop/CoursesShop.vue";
import CourseCards from "./components/shop/CoursesCards.vue";
import BooksShop from "./components/shop/BooksShop.vue";
import ClientsComp from "./components/ClientsComp.vue";
import TestimonialsComp from "./components/TestimonialsComp.vue";

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
</template>

<style lang="scss">
@use "../node_modules/bootstrap/scss/bootstrap.scss" as *;
@use "./assets/styles/general.scss" as *;
@use "./assets/styles/partials/variables" as *;
</style>
