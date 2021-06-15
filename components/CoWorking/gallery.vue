<template>
  <div class="gallery">
    <div class="container gallery-body col justify-content-between">
      <div>
        <span class="cafe-gallery">CAFé ONE GALLERY &nbsp;<img src="@/assets/img/events-marker.svg"
            alt="gallery marker"></span>
        <span class="gallery-text d-flex justify-content-between">
          <h2>Immersive Beautiful<br /> Co-working Space Gallery</h2>
          <img src="@/assets/img/more-events-arrow.svg" alt="more events arrow">
        </span>
      </div>
      <div class="tables text-start">
        <div class="container col pb-5 position-relative pr-0 pl-0">
          <div id="demo" class="carousel slide position-relative" data-ride="carousel">
            <!-- Indicators -->
            <ul class="carousel-indicators">
              <li data-target="#demo" data-slide-to="0" class=""></li>
              <li data-target="#demo" data-slide-to="1" class="active"></li>
              <li data-target="#demo" data-slide-to="2" class=""></li>
            </ul>
            <!-- The slideshow -->
            <div class="carousel-inner">
              <div class="carousel-item active carousel-item-left">
                <div class="d-flex">
                  <div class="col-lg-4 col-sm-12 col-12 d-flex flex-column pl-2 pr-2">
                    <a href="#" class="introduce">
                      <div class="flex-column-1 ">
                        <img src="@/assets/img/cafeone_listing_images.svg" alt="img-1">
                      </div>
                    </a>
                  </div>
                  <div class="col-lg-4 col-sm-12 col-12 d-flex flex-column pl-2 pr-2">
                    <a href="#" class="introduce">
                      <div class="flex-column-1 ">
                        <img src="@/assets/img/cafeone_listing_images.svg" alt="img-2">
                      </div>
                    </a>
                  </div>
                  <div class="col-lg-4 col-sm-12 col-12 d-flex flex-column pl-2 pr-2">
                    <a href="#" class="introduce">
                      <div class="flex-column-1 ">
                        <img src="@/assets/img/cafeone_listing_images.svg" alt="img-3">
                      </div>
                    </a>
                  </div>
                </div>

              </div>
              <div class="carousel-item carousel-item-next carousel-item-left">
                <div class="d-flex justify-content-between">
                  <div class="col-lg-4 col-sm-12 col-12 d-flex flex-column pl-2 pr-2">
                    <a href="#" class="introduce">
                      <div class="flex-column-1 ">
                        <img src="@/assets/img/cafeone_listing_images.svg" alt="img-1">
                      </div>
                    </a>
                  </div>
                  <div class="col-lg-4 col-sm-12 col-12 d-flex flex-column pl-2 pr-2">
                    <a href="#" class="introduce">
                      <div class="flex-column-1 ">
                        <img src="@/assets/img/cafeone_listing_images.svg" alt="img-2">
                      </div>
                    </a>
                  </div>
                  <div class="col-lg-4 col-sm-12 col-12 d-flex flex-column pl-2 pr-2">
                    <a href="#" class="introduce">
                      <div class="flex-column-1 ">
                        <img src="@/assets/img/cafeone_listing_images.svg" alt="img-3">
                      </div>
                    </a>
                  </div>
                </div>
              </div>
              <div class="carousel-item ">
                <div class="d-flex">
                  <div class="col-lg-4 col-sm-12 col-12 d-flex flex-column pl-2 pr-2">
                    <a href="#" class="introduce">
                      <div class="flex-column-1 ">
                        <img src="@/assets/img/cafeone_listing_images.svg" alt="img-1">
                      </div>
                    </a>
                  </div>
                  <div class="col-lg-4 col-sm-12 col-12 d-flex flex-column pl-2 pr-2">
                    <a href="#" class="introduce">
                      <div class="flex-column-1 ">
                        <img src="@/assets/img/cafeone_listing_images.svg" alt="img-2">
                      </div>
                    </a>
                  </div>
                  <div class="col-lg-4 col-sm-12 col-12 d-flex flex-column pl-2 pr-2">
                    <a href="#" class="introduce">
                      <div class="flex-column-1 ">
                        <img src="@/assets/img/cafeone_listing_images.svg" alt="img-3">
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
    name: "gallery",
    data() {
      return {}
    },
  };

</script>
<style lang="scss" scoped>
  @import "@/scss/abstracts/_variables";
  @import "@/scss/abstracts/_mixins";

  .gallery-text {
    font-size: 20px;
    font-weight: normal;
    font-stretch: normal;
    font-style: normal;
    line-height: 1.46;
    letter-spacing: normal;
    color: #9A9A9A;
    display: block;
    text-align: start;
    padding-bottom: 1.5rem;
    margin-right: auto;
    margin-left: 0;
  }

  .gallery {
    margin: 40px 0px 50px;
  }

  .gallery-body {
    width: 1150px;
    margin: auto;
    padding-top: 50px;
    padding-bottom: 20px;
  }

  .gallery-body h2 {
    font-size: 40px;
    font-weight: 800;
    font-stretch: normal;
    font-style: normal;
    line-height: 1.18;
    letter-spacing: normal;
    color: #474E59;
    text-align: start;
  }

  .tables {
    border-radius: 2px;
    margin-bottom: 20px;
  }

  span {
    margin: 10px;
  }

  @media only screen and (max-width: 1150px) {
    .gallery-body {
      display: block;
      align-items: center;
      justify-content: center;
    }

    .gallery-body h2 {
      font-size: 32px;
    }

    .gallery-body p {
      margin-bottom: 70px;
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
    .gallery-body {
      width: 99%;
    }

    .gallery-body p {
      margin-bottom: 30px;
    }
  }

  .cafe-gallery {
    font-style: normal;
    font-weight: 500;
    font-size: 20px;
    line-height: 30px;
    color: #222831;
    margin: 0;
    text-transform: uppercase;
  }

  .introduce {
    height: 22rem;
    background-color: white;
    box-shadow: 0 3px 10px #5969f642;
    color: black;
  }

  .introduce:hover {
    box-shadow: 0 3px 15px #5969f666;
    color: black;
    text-decoration: none;
  }

  .flex-column-1 {
    height: 22rem;
    width: 100%;
  }

  .pic {
    height: 70px;
    width: 70px;
    margin-left: 20px;
    border-radius: 50%;
    transition: all .2s ease-in-out;
  }

  .introduce:hover .pic {
    transform: scale(1.1);
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
    height: 22rem;
  }

</style>
