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
</template>

<style lang="scss">
.big-price {
  font-size: 1.6rem;
}
</style>
