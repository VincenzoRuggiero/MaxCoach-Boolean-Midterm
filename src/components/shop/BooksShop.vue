<script>
import BooksCards from "./BooksCards.vue";
import CTAbutton from "../CTAbutton.vue";

export default {
  name: "BooksShop",
  components: {
    BooksCards,
    CTAbutton,
  },
};
</script>

<template>
  <div>
    <div class="container">
      <div class="row">
        <div class="col-6 left">
          <span class="section-name">Book Store Online</span>
          <h2 class="books-shop-heading my-2">
            Be Alpha With <br />
            <span class="green">Wingman's Book</span>
          </h2>
          <ul class="py-4 grey">
            <li>Help you understand yourself better</li>
            <li>Revealing mature tips</li>
            <li>Give the right advice</li>
            <li>Fascinating examples of alpha man</li>
          </ul>
          <CTAbutton buttonText="Get Free Book" hide="true" />
        </div>
        <div class="col-6 d-flex">
          <BooksCards />
        </div>
      </div>
    </div>
  </div>
</template>

<style lang="scss" scoped>
@use "../../assets/styles/partials/variables" as *;
.left {
  span {
    display: inline-block;
  }

  h2 {
    color: $congress-blue;
  }

  ul li {
    line-height: 2.2rem;
  }

  .books-shop-heading {
    line-height: 3rem;
  }
}
</style>
