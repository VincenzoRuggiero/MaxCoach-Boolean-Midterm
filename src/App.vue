<script>
import HeaderComp from "./components/HeaderComp.vue";
import ResultsComp from "./components/ResultsComp.vue";

export default {
  components: {
    HeaderComp,
    ResultsComp,
  },
};
</script>

<template>
  <HeaderComp />
  <ResultsComp />
</template>

<style lang="scss">
@use "../node_modules/bootstrap/scss/bootstrap.scss" as *;
@use "./assets/styles/general.scss" as *;
@use "./assets/styles/partials/variables" as *;
</style>
