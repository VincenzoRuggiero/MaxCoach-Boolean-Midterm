<script>
export default {
  name: "HeaderComp",
};
</script>

<template>
  <div class="container header">
    <div class="div">
      <img src="../assets/styles/images/dark-logo.png" alt="Site logo" />
    </div>
    <nav>
      <ul>
        <li><a href="">Home</a></li>
        <li><a href="">Pages</a></li>
        <li><a href="">Courses</a></li>
        <li><a href="">Features</a></li>
        <li><a href="">Blog</a></li>
        <li><a href="">Shop</a></li>
      </ul>
    </nav>
    <div class="social-links">
      <span>Twitter</span>
      <span>FB</span>
      <span>IG</span>
      <span>LinkedIn</span>
    </div>
  </div>
</template>

<style lang="scss">
.container {
  width: 80%;
  margin: 0 auto;
}
.header {
  display: flex;
  justify-content: space-between;
  padding-top: 1rem;

  img {
    width: 10rem;
  }

  ul {
    list-style-type: none;

    li {
      display: inline;

      a {
        display: inline-block;
        padding: 0 1rem;
        text-decoration: none;
      }
    }
  }

  .social-links span {
    padding: 0 0.8rem;
  }
}
</style>
