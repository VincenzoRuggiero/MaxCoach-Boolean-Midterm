<script>
export default {
  name: "HeaderComp",
};
</script>

<template>
  <!-- Header  -->
  <div class="background">
    <div class="container header">
      <div class="div">
        <img src="../assets/styles/images/dark-logo.png" alt="Site logo" />
      </div>
      <nav>
        <ul>
          <li><a href="#">Home</a></li>
          <li><a href="#">Pages</a></li>
          <li><a href="#">Courses</a></li>
          <li><a href="#">Features</a></li>
          <li><a href="#">Blog</a></li>
          <li><a href="#">Shop</a></li>
        </ul>
      </nav>
      <div class="social-links">
        <span>Twitter</span>
        <span>FB</span>
        <span>IG</span>
        <span>LinkedIn</span>
      </div>
    </div>

    <!-- Hero Section -->
    <div class="container mt-5">
      <div class="row align-items-center">
        <div class="col-6">
          <span>I'm wingman</span>
          <h1>Peace on Earth A Wonderful Wish But No Way</h1>
          <p>
            Success isn't overnight. It's when everyday you get a little better
            than the day before. It all adds up.
          </p>
          <a href="#">Get Started For Free</a
          ><span class="arrow-icon">&#x2192;</span>
        </div>
        <div class="col-6">
          <img
            class="img-fluid"
            src="../assets/styles/images/home-movation-hero-image.png"
            alt="" />
        </div>
      </div>
    </div>
  </div>
</template>

<style lang="scss">
.background {
  // background-image: url('../assets/styles/images/');
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
