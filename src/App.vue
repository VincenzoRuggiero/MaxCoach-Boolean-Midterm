<script>
import HeaderComp from "./components/HeaderComp.vue";

export default {
  components: {
    HeaderComp,
  },
};
</script>

<template>
  <HeaderComp />
</template>

<style lang="scss">
@use "../node_modules/bootstrap/scss/bootstrap.scss" as *;
@use "./assets/styles/general.scss" as *;
@use "./assets/styles/partials/variables" as *;
</style>
