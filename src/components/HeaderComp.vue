<script>
import CTAbutton from "./CTAbutton.vue";

export default {
  name: "HeaderComp",
  components: {
    CTAbutton,
  },
};
</script>

<template>
  <!-- Header  -->
  <div class="section-background">
    <div class="container header d-flex align-content-center">
      <div>
        <img
          class="logo"
          src="../assets/styles/images/dark-logo.png"
          alt="Site logo" />
      </div>
      <nav>
        <ul>
          <li>
            <a href="#">Home</a>
            <font-awesome-icon
              class="dropdown"
              icon="fa-solid fa-chevron-down" />
          </li>
          <li>
            <a href="#">Pages</a>
            <font-awesome-icon
              class="dropdown"
              icon="fa-solid fa-chevron-down" />
          </li>
          <li>
            <a href="#">Courses</a>
            <font-awesome-icon
              class="dropdown"
              icon="fa-solid fa-chevron-down" />
          </li>
          <li>
            <a href="#">Features</a>
            <font-awesome-icon
              class="dropdown"
              icon="fa-solid fa-chevron-down" />
          </li>
          <li>
            <a href="#">Blog</a>
            <font-awesome-icon
              class="dropdown"
              icon="fa-solid fa-chevron-down" />
          </li>
          <li>
            <a href="#">Shop</a>
            <font-awesome-icon
              class="dropdown"
              icon="fa-solid fa-chevron-down" />
          </li>
        </ul>
      </nav>
      <div class="social-links fs-5">
        <font-awesome-icon class="icon" icon="fa-brands fa-twitter" />
        <font-awesome-icon class="icon" icon="fa-brands fa-facebook-f" />
        <font-awesome-icon class="icon" icon="fa-brands fa-instagram" />
        <font-awesome-icon class="icon" icon="fa-brands fa-linkedin" />
      </div>
    </div>

    <!-- Hero Section -->
    <div class="container mt-5 p-4">
      <div class="row align-items-center">
        <div class="col-12 col-md-6">
          <span class="section-name grey">I'm wingman</span>
          <h1 class="hero-heading">
            Peace on Earth A Wonderful Wish But No Way
          </h1>
          <p class="hero-content">
            Success isn't overnight. It's when everyday you get a little better
            than the day before. It all adds up.
          </p>
          <CTAbutton buttonText="Get Started For Free" />
        </div>
        <div class="col-md-6 d-none">
          <img
            class="img-fluid hero-background"
            src="../assets/styles/images/home-movation-hero-image.png"
            alt="" />
        </div>
      </div>
    </div>
  </div>
</template>

<style lang="scss">
@use "../assets/styles/general.scss" as *;
@use "../assets/styles/partials/variables" as *;
.section-background {
  background-image: url("../assets/styles/images/background-pattern-wavify.png");
  background-color: $athens-grey;

  .hero-background {
    background-image: url("../assets/styles/images/home-movation-shape-face-600x534.png");
    // background-size: cover;
    background-position: bottom;
  }
}

.header {
  display: flex;
  justify-content: space-between;
  padding-top: 1rem;

  .logo {
    width: 10rem;
  }

  nav ul {
    list-style-type: none;

    li {
      display: inline;

      a {
        font-size: 1.2rem;
        display: inline-block;
        padding: 0 1rem;
        text-decoration: none;
        color: $congress-blue;

        &:hover {
          color: $mountain-meadow;
        }
      }

      .dropdown {
        position: relative;
        right: 0.5rem;
      }
    }
  }

  .social-links .icon {
    padding: 0 0.8rem;

    &:hover {
      color: $mountain-meadow;
    }
  }
}

h1.hero-heading {
  font-size: 3rem;
  line-height: 4rem;
  padding: 1.5rem 15rem 1.5rem 0;
}

p.hero-content {
  line-height: 2rem;
  padding: 0 11rem 2rem 0;
  font-weight: lighter;
}
</style>
