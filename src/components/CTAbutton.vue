<script>
export default {
  name: "CTAbutton",
};
</script>

<template>
  <a class="button">Get Started For Free <span class="arrow">&#x2192;</span></a>
</template>

<style lang="scss" scoped>
@use "../assets/styles/partials/variables" as *;

.button {
  color: $white;
  background-color: $mountain-meadow;
  text-decoration: none;
  padding: 0.8rem 3rem;
  font-weight: bold;
  border-radius: 5px;

  .arrow {
    margin-left: 0.7rem;
  }
}
</style>
