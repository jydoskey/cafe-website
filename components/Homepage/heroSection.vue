<template>
  <section class="home-section">
    <div>
      <!-- <div class="row justify-content-center">
        <div class="col-xl-8 col-lg-10">
          <h2 class="heading-2 home-section__title text-center" :class="titleClass">{{ title }}</h2>
          <p class="paragraph home-section__description text-center" :class="descriptionClass"> {{ description }} </p>
        </div>
      </div> -->
      <div id="carouselExampleIndicators" class="carousel slide" data-ride="carousel">
        <ol class="carousel-indicators mr-auto">
          <li data-target="#carouselExampleIndicators" data-slide-to="0" class="active"><img
              src="@/assets/img/carousel/she-can.jpeg" class="d-block w-100">
          </li>
          <li data-target="#carouselExampleIndicators" data-slide-to="1"><img src="@/assets/img/carousel/adaobi.jpeg"
              class="d-block w-100"></li>
          <li data-target="#carouselExampleIndicators" data-slide-to="2"><img
              src="@/assets/img/carousel/braithwathe.jpeg" class="d-block w-100"></li>
          <li data-target="#carouselExampleIndicators" data-slide-to="3"><img src="@/assets/img/carousel/fisayo.jpeg"
              class="d-block w-100"></li>
          <li data-target="#carouselExampleIndicators" data-slide-to="4"><img src="@/assets/img/carousel/adaobi.jpeg"
              class="d-block w-100"></li>
        </ol>
        <!-- <ol class="carousel-indicators">
        <li data-target="#carouselExampleIndicators" data-slide-to="0" class="active"></li>
        <li data-target="#carouselExampleIndicators" data-slide-to="1"></li>
        <li data-target="#carouselExampleIndicators" data-slide-to="2"></li>
        <li data-target="#carouselExampleIndicators" data-slide-to="3"></li>
        <li data-target="#carouselExampleIndicators" data-slide-to="4"></li>
    </ol> -->
        <div class="carousel-inner">
          <div class="carousel-item active">
            <img src="@/assets/img/carousel/she-can.jpeg" class="d-block w-100">
          </div>
          <div class="carousel-item">
            <img src="@/assets/img/carousel/adaobi.jpeg" class="d-block w-100">
          </div>
          <div class="carousel-item">
            <img src="@/assets/img/carousel/braithwathe.jpeg" class="d-block w-100">
          </div>
          <div class="carousel-item">
            <img src="@/assets/img/carousel/fisayo.jpeg" class="d-block w-100">
          </div>
          <div class="carousel-item">
            <img src="@/assets/img/carousel/adaobi.jpeg" class="d-block w-100">
          </div>
        </div>
        <div class="overlay"></div>
      </div>
    </div>
  </section>
</template>

<script>
  export default {
    name: "home-hero",
  }

</script>

<style lang="scss" scoped>
  @import "@/scss/abstracts/_variables";
  @import "@/scss/abstracts/_mixins";

  .container {
    @include breakpoint-min(sm) {
      min-width: 540px;
      max-width: calc(100% - 70px);
    }

    @include breakpoint-min(md) {
      max-width: calc(100% - 108px);
      min-width: 720px;
    }

    @include breakpoint-min(lg) {
      min-width: 960px;
    }

    @media (min-width: 1440px) {
      max-width: 1300px;
    }
  }

  .animate {
    transition-delay: .08s;
    transition-duration: .20s;
    transition-timing-function: ease-in;
  }

  .slide-up {
    transform: translateY(0);
  }

  .slide-up.animate-active {
    transform: translateY(-60px);
  }

  .home-section {
    padding: 0 0 7rem 0;
    background: $white;
  }

  .home-section__title {
    margin-bottom: 1.5rem;
    color: $black;
  }

  .home-section__description {
    margin-bottom: 5rem;
    color: $steel;
  }

  @include breakpoint-min(lg) {
    .home-section {
      padding: 0 0 8rem 0;
    }

    .home-section__description {
      margin-bottom: 6.25rem;
    }

    .heading-2 {
      @include breakpoint-min(sm) {
        font-size: 25px;
      }

      @include breakpoint-min(md) {
        font-size: 30px;
      }

      @include breakpoint-min(lg) {
        font-size: 40px;

      }

      @include breakpoint-min(xl) {
        font-size: 48px;
      }
    }
  }

  .carousel-indicators li {
    width: 150px;
    height: 100%;
    opacity: 1;
  }

  .carousel-item {
    @include breakpoint-min (lg) {
      height: 680px;
    }
  }

  .carousel-item {}

  .overlay {
    position: absolute;
    bottom: 0;
    background: rgb(0, 0, 0);
    background: rgba(0, 0, 0, 0.5);
    /* Black see-through */
    color: #f1f1f1;
    width: 100%;
    height: 100%;
    transition: .5s ease;
    opacity: 0.9;
    color: white;
    font-size: 20px;
    padding: 20px;
    text-align: center;
    z-index: 1;
  }

</style>
