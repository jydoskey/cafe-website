<template>
  <section class="about-section">
    <iframe class="about-video" src="https://www.youtube.com/embed/lTRHnFtFH50" title="YouTube video player"
      frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
      allowfullscreen></iframe>
    <div class="container">
      <div class="row">
        <div class="col-lg-6">
          <div class="about-us">
            <div class="about-text">
              <h2>About Café One</h2>
              <h3>Who we are</h3>
              <p>Nulla porttitor accumsan tincidunt. Curabitur aliquet quam id dui posuere blandit. Curabitur aliquet
                quam
                id dui posuere blandit. Curabitur arcu erat, accumsan id imperdiet et, porttitor at sem.
              </p>
              <h3>What We Do</h3>
              <p>Nulla porttitor accumsan tincidunt. Curabitur aliquet quam id dui posuere blandit. Curabitur aliquet
                quam
                id dui posuere blandit. Curabitur arcu erat, accumsan id imperdiet et, porttitor at sem.
              </p>
              <h3>What Can You Do In Café One</h3>
              <p>Nulla porttitor accumsan tincidunt. Curabitur aliquet quam id dui posuere blandit. Curabitur aliquet
                quam
                id dui posuere blandit. Curabitur arcu erat, accumsan id imperdiet et, porttitor at sem.
              </p>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
  export default {
    name: 'AboutCafeOne',
  }

</script>

<style lang="scss" scoped>
  @import "@/scss/abstracts/_variables";
  @import "@/scss/abstracts/_mixins";

  .about-section {
    position: relative;
    padding-top: 3rem;
    padding-bottom: 3rem;

    @include breakpoint-max (lg) {
      background: rgba($color: grey, $alpha: 0.7);
    }

    @include breakpoint-min (lg) {
      &::before {
        content: '';
        display: block;
        position: absolute;
        top: 0;
        right: 0;
        width: 75%;
        height: 100%;
        background: rgba($color: grey, $alpha: 0.7);
      }
    }
  }

  .about-video {
    width: 75%;
    height: 100%;
    position: absolute;
    top: 0;
    right: 0;

    @include breakpoint-max (lg) {
      width: 100%;
      position: relative;
      height: 50vh;
    }
  }

  .about-us {
    width: 100%;
    height: auto;
    background-position: inherit;
    background-repeat: no-repeat;
    background-size: cover;

    &::after {
      width: 100%;
      height: 60vh;
      z-index: 1;
      background: #474E59;
      position: relative;
      display: block;
      opacity: 0.98;
      content: '';

      @include breakpoint-min (lg) {
        width: 100%;
        height: 35rem;
      }

      @media (max-width:380px) {
        width: 100%;
        height: 125vh;
      }

      @media (max-width:320px) {
        width: 100%;
        height: 155vh;
      }
    }

    @include breakpoint-min (lg) {
      width: 100%;
      height: 35rem;
    }
  }

  .about-text {
    position: absolute;
    z-index: 999;
    display: block;
    color: #ffffff;
    padding: 1.875rem 2.75rem;
    height: auto;
  }

  .about-text h2 {
    font-size: 1.7rem;
  }

  .about-text h3 {
    font-size: 1.25rem;
  }

  .about-text p {
    font-size: 1.00rem;
  }

</style>
