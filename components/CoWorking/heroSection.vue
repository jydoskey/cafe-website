<template>
  <section class="hero-section">
    <div class="container">
      <div class="row">
        <div class="col-lg-5">
          <h1 class="hero-section__header">Interested In <span class="text-red">Working</span><br /> From A
            Creative<br />
            Environment?</h1>
          <p class="hero-section__description">Our Co-working space is for you</p>
          <div class="text-center pt-2">
            <button type="submit" id="submit" name="submit" class="col-8 btn btn-lg btn-block btn-red">
              BOOK A SPACE
            </button>
          </div>
        </div>
        <div class="col-lg-7">
          <div class="hero-image">
            <img class="hero-image" src="@/assets/img/gallery/gallery-3.jpeg">
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
    padding-bottom: 4rem;

    @include breakpoint-min(lg) {
      padding-bottom: 7rem;
    }
  }

  .btn-red {
    border-radius: 0% !important;
    font-size: 16px;
    height: 3.5rem;
    @include breakpoint-max (md) {
      margin: 0 auto;
      margin-bottom: 2rem;
    }
  }

  .hero-image {
    width: 100%;
    height: 20rem;
    background-position: inherit;
    background-repeat: no-repeat;
    background-size: cover;

    @include breakpoint-min(lg) {
      top: 3rem;
      position: relative;
      width: 100%;
      max-width: 720px;
      height: 26rem;
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
      width: 40rem;
    }

    @include breakpoint-max(lg) {
      text-align: center;
    }
  }

  .hero-section__description {
    text-align: start;
    font-family: Lato;
    font-style: normal;
    font-weight: 500;
    font-size: 20px;
    line-height: 30px;
    color: #6A6A6A;

    @include breakpoint-max(lg) {
      text-align: center;
    }
  }

</style>
