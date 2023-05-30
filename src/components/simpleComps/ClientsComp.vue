<script>
export default {
  name: "ClientsComp",
  data() {
    return {
      logos: [
        {
          img: "logo-01",
        },
        {
          img: "logo-02",
        },
        {
          img: "logo-03",
        },
        {
          img: "logo-04",
        },
        {
          img: "logo-05",
        },
        {
          img: "logo-06",
        },
      ],
    };
  },
  methods: {
    getImagePath(image) {
      return new URL(
        `../../assets/styles/images/client-${image}-primary.png`,
        import.meta.url
      ).href;
    },
  },
};
</script>

<template>
  <div class="container my-5 py-2">
    <div class="row">
      <div class="col-2" v-for="logo in logos">
        <img
          class="img-fluid logo"
          :src="getImagePath(logo.img)"
          alt="Client logo" />
      </div>
    </div>
  </div>
</template>

<style lang="scss">
.logo {
  opacity: 0.5;

  &:hover {
    transition: all 0.2s ease-in;
    opacity: 1;
  }
}
</style>
