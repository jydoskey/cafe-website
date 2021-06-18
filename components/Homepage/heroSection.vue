<template>
  <section class="home-section">
    <div id="carouselExampleIndicators" class="carousel slide" data-ride="carousel">
      <div class="carousel-indicators-group">
        <ol class="carousel-indicators">
          <li data-target="#carouselExampleIndicators" data-slide-to="0" class="active">
            <img src="@/assets/img/gallery/gallery-1.jpeg" class="d-block w-100">
          </li>
          <li data-target="#carouselExampleIndicators" data-slide-to="1">
            <img src="@/assets/img/gallery/carousel-yoga.jpeg" class="d-block w-100">
          </li>
          <li data-target="#carouselExampleIndicators" data-slide-to="2">
            <img src="@/assets/img/gallery/gallery-3.jpeg" class="d-block w-100">
          </li>
          <li data-target="#carouselExampleIndicators" data-slide-to="3">
            <img src="@/assets/img/gallery/service-magic.png" class="d-block w-100">
          </li>
        </ol>
        <ol class="carousel-progress">
          <a class="carousel-control-prev" href="#carouselExampleIndicators" role="button" data-slide="prev">
            <img src="@/assets/img/carousel/previous.svg" alt="" aria-hidden="true">
            <span class="sr-only">Previous</span>
          </a>
          <div class="lists">
            <li data-target="#carouselExampleIndicators" data-slide-to="0" class="active"></li>
            <li data-target="#carouselExampleIndicators" data-slide-to="1"></li>
            <li data-target="#carouselExampleIndicators" data-slide-to="2"></li>
            <li data-target="#carouselExampleIndicators" data-slide-to="3"></li>
          </div>
          <a class="carousel-control-next" href="#carouselExampleIndicators" role="button" data-slide="next">
            <img src="@/assets/img/carousel/next.svg" alt="" aria-hidden="true">
            <span class="sr-only">Next</span>
          </a>
        </ol>
      </div>
      <div class="carousel-inner">
        <div class="carousel-item active">
          <img src="@/assets/img/gallery/gallery-1.jpeg" class="d-block w-100">
          
          <div class="carousel-caption">
            <h2 class="heading-2 home-section__title">
              Catchy Headline About Slider Item
            </h2>
            <p class="paragraph">
              Text about this particular item comes here. The image is also in the background. The CTA is not necessary
            </p>
            <p>
              10 April 10am - 2pm
            </p>
            <button class="btn btn-danger">REGISTER</button>
          </div>
        </div>
        <div class="carousel-item">
          <img src="@/assets/img/gallery/carousel-yoga.jpeg" class="d-block w-100">

          <div class="carousel-caption">
            <h2 class="heading-2 home-section__title">
              Catchy Headline About Slider Item
            </h2>
            <p class="paragraph">
              Text about this particular item comes here. The image is also in the background. The CTA is not necessary
            </p>
            <p>
              10 April 10am - 2pm
            </p>
            <button class="btn btn-danger">REGISTER</button>
          </div>
        </div>
        <div class="carousel-item">
          <img src="@/assets/img/gallery/gallery-3.jpeg" class="d-block w-100">

          <div class="carousel-caption">
            <h2 class="heading-2 home-section__title">
              Catchy Headline About Slider Item
            </h2>
            <p class="paragraph">
              Text about this particular item comes here. The image is also in the background. The CTA is not necessary
            </p>
            <p>
              10 April 10am - 2pm
            </p>
            <button class="btn btn-danger">REGISTER</button>
          </div>
        </div>
        <div class="carousel-item">
          <img src="@/assets/img/gallery/service-magic.png" class="d-block w-100">

          <div class="carousel-caption">
            <h2 class="heading-2 home-section__title">
              Catchy Headline About Slider Item
            </h2>
            <p class="paragraph">
              Text about this particular item comes here. The image is also in the background. The CTA is not necessary
            </p>
            <button class="btn btn-danger">REGISTER</button>
          </div>
        </div>
      </div>
      <div class="overlay"></div>
    </div>
  </section>
</template>

<script>
  export default {
    name: "event-hero",
    mounted() {
      let _addClass = $.fn.addClass;

      $.fn.addClass = function () {
        let activeLI = document.querySelector(".carousel-indicators > .active");
        if (activeLI) {
          activeLI = activeLI.getAttribute('data-slide-to');
          let target = document.querySelectorAll(".carousel-progress li");
          let lists = document.querySelectorAll(".carousel-progress li");
          for (const item of lists) {
            item.classList.remove('active');
          }
          target[activeLI].classList.add('active');
        }
        return _addClass.apply(this, arguments);
      }
    }
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

  .carousel.slide, .carousel-inner, .carousel-item, .carousel-inner img {
    height: 660px;
    @include breakpoint-max (md) {
      height: 550px;
    }
  }

  .carousel-inner img {
    object-fit: cover;
  }

  .carousel-caption {
    width: 680px;
    max-width: 95%;
    padding: 0 0 80px 80px;
    right: 0;
    left: 0;
    text-align: left;
    @include breakpoint-max(xl) {
      padding: 0 0 60px 60px;
    }
    @include breakpoint-max(lg) {
      padding: 0 0 30px 0;
      right: unset;
      left: 50%;
      transform: translateX(-50%);
      bottom: 180px;
    }
    @include breakpoint-max(md) {
      bottom: 120px;
    }
  }

  .carousel-caption h2 {
    font-family: Lora;
    font-weight: bold;
    font-size: 52px;
    line-height: 1.29;
    margin-bottom: 15px;
    @include breakpoint-max(lg) {
      font-size: 40px;
      max-width: 95%;
      margin: 0 auto 15px auto;
    }
    @include breakpoint-max(md) {
      max-width: 512px;
    }
    @include breakpoint-max(sm) {
      font-size: 35px;
      max-width: 400px;
    }
    @include breakpoint-max(xs) {
      font-size: 28px;
      max-width: unset;

    }
  }

  .carousel-caption p {
    max-width: 400px;
    width: 100%;
    font-family: Lato;
    font-weight: 500;
    font-size: 20px;
    line-height: 1.5;
    margin-bottom: 12px;
    @include breakpoint-max(xl) {
      max-width: 350px;
    }
    @include breakpoint-max(lg) {
      font-size: 16px;
      margin: 0 auto 16px auto;;
    }
    @include breakpoint-max(xs) {
      max-width: 95%;
    }
  }

  .carousel-caption h2, .carousel-caption p {
    color: #ffffff;
    text-align: left;
    @include breakpoint-max(lg) {
      text-align: center;
    }
  }

  .carousel-caption .event-category {
    font-weight: 400;
    margin-bottom: 0;
  }

  .carousel-caption button.btn-danger {
    margin-top: 40px;
    width: 340px;
    height: 63px;
    background-color: #BC2934;
    border-radius: 0;
    @include breakpoint-max(lg) {
      display: block;
      width: 250px;
      height: 55px;
      margin: 20px auto 0 auto;
    }
  }

  .carousel-indicators-group {
    position: absolute;
    bottom: 3.5rem;
    z-index: 2;
    right: 0;
    display: flex;
    overflow: hidden;
    flex-direction: column;
    @include breakpoint-max(lg) {
      right: unset;
      left: 50%;
      transform: translateX(-50%);
      bottom: 0.5rem;
    }
  }

  .carousel-indicators {
    margin-right: -100px;
    margin-left: 0;
    position: static;
    @include breakpoint-max(lg) {
      margin-right: 0;
    }
  }

  .carousel-indicators li {
    width: 134px;
    height: 120px;
    opacity: 1;
    margin: 0 5px;
    @include breakpoint-max(xl) {
      width: 120px;
      height: 107px;
    }
    @include breakpoint-max(lg) {
      width: 100px;
      height: 90px;
    }
    @include breakpoint-max(md) {
      width: 50px;
      height: 45px;
    }
  }

  .carousel-indicators li .indicator-text {
    position: absolute;
    width: 100%;
    bottom: 0;
    height: fit-content;
    z-index: 1;
    padding: 0 10px;
    @include breakpoint-max(lg) {
      display: none;
    }
  }

  .carousel-indicators li p {
    font-family: Lora;
    font-size: 14px;
    line-height: 18px;
    letter-spacing: -0.06em;
    color: #FFFFFF;
    margin-bottom: 6px;
  }

  .carousel-indicators li h6 {
    font-family: Lora;
    color: #ffffff;
    font-size: 16px;
    font-weight: 500;
    letter-spacing: -0.06em;
  }

  .carousel-indicators li img {
    object-fit: cover;
    height: 100%;
    width: 100%;
  }

  .carousel-progress {
    align-self: center;
    display: flex;
    align-items: center;
  }

  .carousel-progress {
    padding: 0;
  }

  .carousel-progress .lists {
    display: flex;
    justify-content: center;
    align-items: center;
    height: 3px;
    background-color: rgba(255, 255, 255, 0.66);
    width: 257px;
    margin: 0 24px;
    @include breakpoint-max(md) {
      width: 150px;
    }
  }

  .carousel-progress a img {
    @include breakpoint-max (md) {
      width: 30px;
    }
  }

  .carousel-progress li {
    width: 60px;
    height: 3px;
    list-style: none;
    @include breakpoint-max(md) {
      width: 30px;
    }
  }

  .carousel-progress li.active {
    background-color: #BC2934;
  }

  .carousel-control-prev, .carousel-control-next {
    position: static;
    width: fit-content;
  }



  .overlay {
    position: absolute;
    bottom: 0;
    background: rgba(0, 0, 0, 0.5);
    width: 100%;
    height: 100%;
    z-index: 1;
  }

</style>
