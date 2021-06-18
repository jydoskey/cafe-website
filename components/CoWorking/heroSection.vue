<template>
  <section class="hero-section">
    <div class="container">
      <div class="row">
        <div class="col-lg-5">
          <h1 class="hero-section__header">Interested In <span class="text-red">Working</span> From A Creative
            Environment?</h1>
          <p class="text-steel hero-section__description">Our Co-working space is for you</p>
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
  }

  .hero-image {
    width: 100%;
    height: 20rem;
    background-position: inherit;
    background-repeat: no-repeat;
    background-size: contain;

    @include breakpoint-min(lg) {
      top: 3rem;
      position: relative;
      width: 100%;
      height: 25rem;
    }
  }

  .hero-section__header {
    margin-bottom: 2.5rem;
    text-align: center;

    @include breakpoint-min(lg) {
      text-align: start;
      margin-bottom: 3rem;
    }
  }

  .hero-section__description {
    margin-bottom: 4rem;
    text-align: center;

    @include breakpoint-min(lg) {
      margin-bottom: 7rem;
      text-align: start;
    }
  }

</style>
