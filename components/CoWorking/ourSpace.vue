<template>
  <div class="our-space">
    <div class="container our-space-body col ">
      <div class="space-header justify-content-between align-items-center">
        <h2>Our Space</h2>
        <span class="our-space-text">
          Some text about events come here. Some text<br /> about events come here
        </span>
        <img src="@/assets/img/more-events-arrow.svg" alt="more events arrow">
      </div>
      <div class="tables text-start">
        <div class="container col pb-5 position-relative pr-0 pl-0">
          <div id="demo" class="carousel slide position-relative" data-ride="carousel">
            <ul class="carousel-indicators">
              <li data-target="#demo" data-slide-to="" class=""></li>
              <li data-target="#demo" data-slide-to="1" class="active"></li>
              <li data-target="#demo" data-slide-to="" class=""></li>
            </ul>
            <div class="carousel-inner">
              <div class="carousel-item carousel-item-next carousel-item-left">
                <div class="space-header justify-content-between">
                  <div class="col-lg-4 col-sm-12 col-12 d-flex flex-column p-2 pb-3">
                    <a href="#" class="introduce">
                      <div class="flex-column-1 ">
                        <img src="@/assets/img/gallery/gallery-4.jpeg" alt="img-1">
                      </div>
                      <div class="flex-column-2-red align-items-center bg-black">
                        <div class="register text-center">
                          Available
                        </div>
                      </div>
                      <p class="space-type pt-4">Private Space</p>
                      <p class="space-feature">Feature 1</p>
                      <p class="space-feature">Feature 2</p>
                      <p class="space-feature pb-3">Feature 3</p>
                      <div class="flex-column-2-red align-items-center">
                        <div class="register text-center text-white">
                          Book
                        </div>
                      </div>
                    </a>
                  </div>
                  <div class="col-lg-4 col-sm-12 col-12 d-flex flex-column p-2 pb-3">
                    <a href="#" class="introduce">
                      <div class="flex-column-1 ">
                        <img src="@/assets/img/custom-office.png" alt="img-2">
                      </div>
                      <div class="flex-column-2-red align-items-center bg-black">
                        <div class="register text-center text-red">
                          Coming Soon
                        </div>
                      </div>
                      <p class="space-type pt-4">Custom Office</p>
                      <p class="space-feature">Feature 1</p>
                      <p class="space-feature">Feature 2</p>
                      <p class="space-feature pb-3">Feature 3</p>
                      <div class="flex-column-2-grey align-items-center">
                        <div class="register text-center text-white">
                          Book
                        </div>
                      </div>
                    </a>
                  </div>
                  <div class="col-lg-4 col-sm-12 col-12 d-flex flex-column p-2 pb-3">
                    <a href="#" class="introduce">
                      <div class="flex-column-1 ">
                        <img src="@/assets/img/work-teams.png" alt="img-3">
                      </div>
                      <div class="flex-column-2-red align-items-center bg-black">
                        <div class="register text-center text-red">
                          Coming Soon
                        </div>
                      </div>
                      <p class="space-type pt-4">Working with team</p>
                      <p class="space-feature">Feature 1</p>
                      <p class="space-feature">Feature 2</p>
                      <p class="space-feature pb-3">Feature 3</p>
                      <div class="flex-column-2-grey align-items-center">
                        <div class="register text-center text-white">
                          Book
                        </div>
                      </div>
                    </a>
                  </div>
                </div>
              </div>

            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>
<script>
  export default {
    name: "ourspace",
  };

</script>
<style lang="scss" scoped>
  @import "@/scss/abstracts/_variables";
  @import "@/scss/abstracts/_mixins";

  .our-space-text {
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

  .our-space {
    margin: 40px 0px 0;
  }

  .our-space-body {
    width: 1150px;
    margin: auto;
    padding-bottom: 20px;
  }

  .our-space-body h2 {
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

  .space-header span {
    margin: 10px;
  }

  @media only screen and (max-width: 1150px) {
    .our-space-body {
      display: block;
      align-items: center;
      justify-content: center;
    }

    .our-space-body h2 {
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
    .our-space-body {
      width: 99%;
    }
  }

  .introduce {
    height: 39.4rem;
    background-color: white;
    color: black;
  }

  .introduce:hover {
    box-shadow: 0 3px 15px #5969f666;
    color: black;
    text-decoration: none;
  }

  .flex-column-1 {
    height: 21rem;
    width: 100%;
  }

  .flex-column-2-red {
    height: 3.5rem;
    width: 100%;
    align-items: center;
    background-color: #BC2934;
    padding-top: 0.8rem;
  }

  .flex-column-2-grey {
    height: 3.5rem;
    width: 100%;
    align-items: center;
    background: rgba(188, 41, 52, 0.5);
    padding-top: 0.8rem;
  }

  .carousel-indicators .active {
    background-color: #BC2934;
    ;
  }

  .carousel-indicators li {
    background-color: #c8e5ff;
  }

  .carousel-indicators {
    bottom: -50px;
  }

  .flex-column-1 img {
    width: 100%;
    height: 21rem;
  }

  .register {
    width: 100%;
    font-family: Lato;
    font-style: normal;
    font-weight: bold;
    font-size: 20px;
    line-height: 30px;
    color: #FFE6BA;
  }

  .register img {
    width: 2.241875rem;
    height: 0.636875rem;
  }

  .space-header {
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

  .space-type {
    font-family: Lato;
    font-style: normal;
    font-weight: bold;
    font-size: 20px;
    line-height: 24px;
    color: #222831;
    padding-left: 1rem;
    padding-top: 1rem;
  }

  .space-feature {
    font-family: Lato;
    font-style: normal;
    font-weight: 500;
    font-size: 20px;
    line-height: 18px;
    color: #9A9A9A;
    padding-left: 1rem;
  }

</style>
