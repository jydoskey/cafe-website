<template>
  <div class="features">
    <div class="container features-body col ">
      <div class="features-header justify-content-between align-items-center">
        <div>
          <span class="features-span">FEATURES &nbsp;<img src="@/assets/img/events-marker.svg"
              alt="event marker"></span>
          <h2>Some General Info About<br /> Café One Features</h2>
        </div>
        <span class="features-text">
          Some info about each feature comes here and changes<br /> as the slider moves to each feature. The picture
          changes<br /> too
        </span>
      </div>
      <div class="tables text-start">
        <div class="container col pb-5 position-relative pr-0 pl-0">

        </div>
      </div>
    </div>
  </div>
</template>
<script>
  export default {
    name: "features",
  };

</script>
<style lang="scss" scoped>
  @import "@/scss/abstracts/_variables";
  @import "@/scss/abstracts/_mixins";

  .features-text {
    font-size: 20px;
    font-weight: normal;
    font-stretch: normal;
    font-style: normal;
    line-height: 1.46;
    letter-spacing: normal;
    color: #9A9A9A;
    text-align: start;
    font-family: Lato;
    margin-left: 0;
  }

  .features {
    margin: 40px 0px 0;
  }

  .features-body {
    width: 1150px;
    margin: auto;
    padding-top: 50px;
    padding-bottom: 20px;
  }

  .features-body h2 {
    font-size: 40px;
    font-weight: 800;
    font-stretch: normal;
    font-style: normal;
    line-height: 1.18;
    letter-spacing: normal;
    color: #474E59;
    text-align: start;
    font-family: Lora;
  }

  .tables {
    border-radius: 2px;
    margin-bottom: 20px;
  }

  @media only screen and (max-width: 1150px) {
    .features-body {
      display: block;
      align-items: center;
      justify-content: center;
    }

    .features-body h2 {
      font-size: 32px;
    }

    .tables {
      width: 100%;
      height: auto;
      border-radius: 2px;
      background-color: #ffffff;
      margin-bottom: 20px;
      display: inline-block;
      align-items: center;
      justify-content: center;
      margin-top: 4rem;
    }

  }

  @media only screen and (max-width: 1150px) {
    .features-body {
      width: 99%;
    }
  }

  .features-header {
    display: block;
    padding-bottom: 3rem;

    @include breakpoint-min (md) {
      display: flex;
    }
  }

  .bg-black {
    background-color: #010101;
  }

  .text-red {
    color: #BC2934;
  }

  .features-type {
    font-family: Lato;
    font-style: normal;
    font-weight: bold;
    font-size: 20px;
    line-height: 24px;
    color: #222831;
    padding-left: 1rem;
    padding-top: 1rem;
  }

  .features-feature {
    font-family: Lato;
    font-style: normal;
    font-weight: 500;
    font-size: 20px;
    line-height: 18px;
    color: #9A9A9A;
    padding-left: 1rem;
  }

  .features-span {
    font-style: normal;
    font-weight: 500;
    font-size: 20px;
    line-height: 30px;
    color: #222831;
    margin: 0rem;
    font-family: Lato;
  }

</style>
