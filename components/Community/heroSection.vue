<template>
  <section class="hero-section">
    <div class="container">
      <div class="row">
        <div class="col-lg-5 header-text">
          <h1 class="hero-section__header">Welcome To Café<br /><span class="text-red">One Community</span></h1>
          <p class="hero-section__description">Some info about community comes here. Nulla port accumsan tincidunt. Cura
            aliquet quam id dui posuere blandi
          </p>
        </div>
        <div class="col-lg-7">
          <div class="hero-image">
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
  export default {
    methods: {},
  }

</script>

<style lang="scss" scoped>
  @import "@/scss/abstracts/_variables";
  @import "@/scss/abstracts/_mixins";

  .hero-section {
    position: relative;
    padding-top: 9rem;
  }

  .header-text {
    @include breakpoint-min (lg) {
      top: 5rem;
    }
  }

  .hero-image {
    width: 100%;
    height: 20rem;
    background-position: inherit;
    background-repeat: no-repeat;
    background-size: cover;
    background-image: url("@/assets/img/community-mobile.png");

    @include breakpoint-min(lg) {
      top: -9rem;
      right: -4rem;
      position: relative;
      width: 100%;
      max-width: 842px;
      background-image: url("@/assets/img/community-header.svg");
      height: 720px;
    }
  }

  .col-lg-7 {
    @include breakpoint-min (lg) {
      padding: 0;
    }
  }

  .hero-section__header {
    margin-bottom: 2.5rem;
    font-family: Lora;
    font-style: normal;
    font-weight: bold;
    font-size: 3.25rem;
    line-height: 67px;
    color: #474E59;

    @include breakpoint-min(lg) {
      text-align: start;
      position: relative;
      margin-bottom: 3rem;
    }

    @include breakpoint-max(lg) {
      text-align: center;
    }
  }

  .hero-section__description {
    font-family: Lato;
    font-style: normal;
    font-weight: 500;
    font-size: 20px;
    line-height: 30px;
    color: #6A6A6A;

    @include breakpoint-min(lg) {
      text-align: start;
      position: relative;
    }
  }

  .col-lg-5,
  .col-lg-7 {
    @include breakpoint-min (lg) {
      height: 630px;
    }
  }

</style>
