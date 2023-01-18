<script>
import HeaderComp from "./components/HeaderComp.vue";
import ResultsComp from "./components/ResultsComp.vue";
import PresentationComp from "./components/PresentationComp.vue";

export default {
  components: {
    HeaderComp,
    ResultsComp,
    PresentationComp,
  },
};
</script>

<template>
  <HeaderComp />
  <ResultsComp />
  <PresentationComp />
</template>

<style lang="scss">
@use "../node_modules/bootstrap/scss/bootstrap.scss" as *;
@use "./assets/styles/general.scss" as *;
@use "./assets/styles/partials/variables" as *;
</style>
