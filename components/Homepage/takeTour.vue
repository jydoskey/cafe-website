<template>
  <section>
    <div class="take-tour">
      <div class="container">
        <div class="row take-tour-content pb-4">
          <div class="col-xl-5 col-lg-5 header">
            <h2 class="contact-section__title header-text">
              Take A Tour Take A Tour Take A Tour
            </h2>
            <p class="header-p">
              Some text comes here about taking a tour. Some text comes here about taking a tour
            </p>
            <button type="submit" id="submit" name="submit" class="col-md-8 btn btn-lg btn-block btn-red">
              TAKE A TOUR
            </button>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>
<script>
  export default {
    name: "takeTour",
  };

</script>
<style lang="scss" scoped>
  @import "@/scss/abstracts/_variables";
  @import "@/scss/abstracts/_mixins";

  .btn-red {
    border-radius: 0% !important;
    font-size: 16px;
    height: 3rem;
    margin-top: 2.5rem;
    margin-bottom: 8.125rem;
  }

  .take-tour {
    background-image: url("@/assets/img/taketour.svg");
    margin: 40px auto 0px;
    padding-bottom: 2rem;
    width: 100%;
    height: auto;
    object-fit: contain;
    background-repeat: no-repeat;
    background-size: cover;
  }

  .take-tour-content {
    @include breakpoint-max (md) {
      justify-content: center;
    }
  }

  .header-text {
    font-size: 40px;
    font-weight: bold;
    margin-top: 7rem;
    color: white;
    text-align: left;
    line-height: 1.24;
    letter-spacing: 1.17px;

    @include breakpoint-max (md) {
      text-align: center;
    }
  }

  .header-p {
    margin: 0 auto;
    font-size: 18px;
    font-weight: 800;
    font-stretch: normal;
    font-style: normal;
    line-height: 1.56;
    letter-spacing: normal;
    text-align: start;
    color: #ffffff;

    @include breakpoint-max (md) {
      text-align: center;
    }
  }

  @media only screen and (max-width: 1000px) {

    .header {
      position: relative;
      top: 40px;
    }

    .header-p {
      width: 90%;
      margin: auto;
      height: 56px;
    }
  }

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

</style>
