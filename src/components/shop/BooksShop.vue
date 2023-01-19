<script>
import BooksCards from "./BooksCards.vue";

export default {
  name: "BooksShop",
  components: {
    BooksCards,
  },
};
</script>

<template>
  <div>
    <div class="container">
      <div class="row">
        <div class="col-6">
          <span>Book Store Online</span>
          <h2>
            Be Alpha With <br />
            <span>Wingman's Book</span>
          </h2>
          <ul>
            <li>Help you understand yourself better</li>
            <li>Revealing mature tips</li>
            <li>Give the right advice</li>
            <li>Fascinating examples of alpha man</li>
          </ul>
        </div>
        <div class="col-6 d-flex">
          <BooksCards />
        </div>
      </div>
    </div>
  </div>
</template>

<style lang="scss"></style>
