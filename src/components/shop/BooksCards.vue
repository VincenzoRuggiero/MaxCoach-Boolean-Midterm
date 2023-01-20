<script>
export default {
  name: "BooksCards",
  data() {
    return {
      cardContent: [
        {
          img: "product-book-10-400x400.jpg",
          title: "Alpha man by Maxcoach",
          price: 29,
        },
        {
          img: "product-book-11-400x400.jpg",
          title: "Real man 4.0 by Maxcoach",
          price: 29,
        },
      ],
    };
  },
  methods: {
    getImagePath(image) {
      return new URL(`../../assets/styles/images/${image}`, import.meta.url)
        .href;
    },
  },
};
</script>

<template>
  <div class="book-card text-center" v-for="content in cardContent">
    <img
      class="img-fluid"
      :src="getImagePath(content.img)"
      :alt="content.title" />
    <h6>{{ content.title }}</h6>
    <h5 class="card-price green"><span class="big-price">$30</span>.00</h5>
  </div>
  <div class="options d-flex flex-column">
    <div class="option">
      <font-awesome-icon class="icon" icon="fa-solid fa-magnifying-glass" />
    </div>
    <div class="option">
      <font-awesome-icon class="icon" icon="fa-solid fa-cart-shopping" />
    </div>
    <div class="option">
      <font-awesome-icon class="icon" icon="fa-regular fa-heart" />
    </div>
    <div class="option">
      <font-awesome-icon class="icon" icon="fa-solid fa-signal" />
    </div>
  </div>
</template>

<style lang="scss">
.book-card:hover {
  transition: all 1.5s cubic-bezier(0, 0, 0.2, 1);
  transform: scale3d(1.1, 1.1, 1.1);
}

.big-price {
  font-size: 1.6rem;
}

.options {
  align-items: center;

  .option {
    position: relative;
    top: 3rem;
    right: 3rem;
    background-color: #ffffff;
    border-radius: 50%;
    font-size: 1rem;
    margin-bottom: 10px;

    &:hover {
      transition: all 0.2s ease-in-out;
      box-shadow: rgba(0, 0, 0, 0.19) 0px 10px 20px,
        rgba(0, 0, 0, 0.23) 0px 6px 6px;
    }

    .icon {
      padding: 15px;
    }
  }
}
</style>
