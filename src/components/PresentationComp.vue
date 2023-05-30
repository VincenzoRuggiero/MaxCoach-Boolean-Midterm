<script>
export default {
  name: "PresentationComp",
};
</script>

<template>
  <div class="container">
    <div class="row d-flex align-items-center py-2">
      <div class="col-12 col-md-6 left">
        <span class="section-name green">About Me</span>
        <h2 class="about-heading">
          How to Be an Alpha Male: The 15 Habits of True Alphas
        </h2>
      </div>
      <div class="col-12 col-md-6 right">
        <h5 class="pt-5">
          Want to learn how to be <span class="green">an alpha male</span>? How
          to be more masculine? How to be the man you've always wanted to be?
        </h5>
        <p class="grey">
          Your goal is to show the consistency of business, core values, and
          customer care. Punctuality, responsability, individuality, accuracy,
          enthusiasm - you have to clearly explain how these qualities are
          applicable to your work. And the important thing is you do love what
          you do.
        </p>
      </div>
    </div>
    <div class="row py-5">
      <div class="col-12 col-md-6 embed">
        <img
          class="img-fluid video-embed"
          src="../assets/styles/images/home-movation-video-poster-670x450.jpg"
          alt="" />
      </div>
      <div class="col-12 col-md-6 right">
        <h2>
          "Every morning you have two choices: continue to sleep with your
          dreams, or wake up and chase them."
        </h2>
        <img
          class="glyph"
          src="../assets/styles/images/home-movation-shape-01.png"
          alt="" />
        <h4 class="pt-3">Kaixa Stark</h4>
        <span class="section-name">Wingman</span>
      </div>
    </div>
  </div>
</template>

<style lang="scss" scoped>
span.section-name.green {
  margin-bottom: 4rem;
}
.right {
  padding: 3rem;

  h2 {
    font-size: 2rem;
    margin-right: 4rem;
    line-height: 3.5rem;
  }

  .glyph {
    margin-top: 1.5rem;
  }
}

.about-heading {
  padding-top: 3rem;
  padding-right: 6rem;
  line-height: 4rem;
  font-size: 3rem;
}

.right h5 {
  font-size: 1.2rem;
}
.right p {
  font-size: 1rem;
}

.embed {
  position: relative;

  .video-embed {
    object-fit: cover;
  }

  .play-icon {
    width: 18%;
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
  }
}
</style>
