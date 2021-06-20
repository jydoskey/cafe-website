<template>
  <section class="hero-section">
    <div class="container">
      <div class="row">
        <div class="col-lg-12">
          <h1 class="hero-section__header">Welcome to Café One Café</h1>
          <p class="hero-section__description">Some info about community comes here. Nulla porttitor<br /> accumsan
            tincidunt.
            Curabitur aliquet quam id dui<br /> posuere blandit. Curabitur aliquet quam id dui posuere<br /> blandit.
            Curabitur arcu
            erat, accumsan id imperdiet et,<br /> porttitor at sem.
          </p>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
  export default {}

</script>

<style lang="scss" scoped>
  @import "@/scss/abstracts/_variables";
  @import "@/scss/abstracts/_mixins";

  .hero-section {
    position: relative;
    padding-top: 9rem;
    padding-bottom: 6rem;
    background: url("@/assets/img/cafe-home.png");
    width: 100%;
    height: 100%;
    object-fit: cover;
    color: #FFFFFF;

    @include breakpoint-min(lg) {
      padding-bottom: 7rem;
    }
  }

  .hero-section__header {
    padding-top: 3rem;
    margin-bottom: 2.5rem;
    font-family: Lora;
    font-style: normal;
    font-weight: bold;
    font-size: 3.25rem;
    line-height: 67px;
    color: #FFFFFF;
    z-index: 9999;
    text-align: center;

    @include breakpoint-min(lg) {
      position: relative;
      margin-bottom: 3rem;
    }
  }

  .hero-section__description {
    text-align: center;
    font-family: Lato;
    font-style: normal;
    display: block;
    font-weight: 500;
    font-size: 20px;
    line-height: 30px;
    color: #FFFFFF;
    z-index: 9999;
  }

</style>
