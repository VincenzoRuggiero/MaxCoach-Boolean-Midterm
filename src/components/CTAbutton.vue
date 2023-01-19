<script>
export default {
  name: "CTAbutton",
  props: {
    buttonText: {
      type: String,
      default: () => "Cliccami",
    },
    hide: false,
  },
};
</script>

<template>
  <button class="button">
    {{ buttonText }}<span v-if="!hide" class="arrow">&#x2192;</span>
  </button>
</template>

<style lang="scss" scoped>
@use "../assets/styles/partials/variables" as *;

button {
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
