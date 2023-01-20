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
          <ul class="py-4 grey fa-ul">
            <li>
              <font-awesome-icon
                class="icon green"
                icon="fa-solid fa-check" />Help you understand yourself better
            </li>
            <li>
              <font-awesome-icon
                class="icon green"
                icon="fa-solid fa-check" />Revealing mature tips
            </li>
            <li>
              <font-awesome-icon
                class="icon green"
                icon="fa-solid fa-check" />Give the right advice
            </li>
            <li>
              <font-awesome-icon
                class="icon green"
                icon="fa-solid fa-check" />Fascinating examples of alpha man
            </li>
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

  ul {
    list-style: none;
    margin: 0 0 1rem 0;
    padding: 0 1rem 0 0;

    .icon {
      margin-right: 1rem;
    }

    li {
      line-height: 2.2rem;
    }
  }

  .books-shop-heading {
    line-height: 3rem;
  }
}
</style>
