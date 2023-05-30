<script>
export default {
  name: "ResultsComp",
  data() {
    return {
      results: [
        {
          data: "1.926",
          category: "Finished Sessions",
        },
        {
          data: "100%",
          category: "Satisfaction Rate",
        },
        {
          data: "3092+",
          category: "Enrolled Learners",
        },
        {
          data: "200",
          category: "Online Instructors",
        },
      ],
    };
  },
};
</script>

<template>
  <div class="container my-5 py-5">
    <div class="row text-center">
      <div class="col-6 col-md-3" v-for="result in results">
        <h3 class="green">{{ result.data }}</h3>
        <p class="grey">{{ result.category.toUpperCase() }}</p>
      </div>
    </div>
  </div>
</template>

<style lang="scss"></style>
