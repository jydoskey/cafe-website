<template>
  <section class="pt-5 circle-1">
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
                    <img src="@/assets/img/event-1.jpeg" alt="img-1">
                  </div>
                  <div class="flex-column-2-red">

                  </div>
                </a>
              </div>
              <div class="col-lg-4 col-sm-12 col-12 d-flex flex-column pl-2 pr-2">
                <a href="#" class="introduce">
                  <div class="flex-column-1 ">
                    <img src="@/assets/img/event-2.jpeg" alt="img-2">
                  </div>
                  <div class="flex-column-2-grey">

                  </div>
                </a>
              </div>
              <div class="col-lg-4 col-sm-12 col-12 d-flex flex-column pl-2 pr-2">
                <a href="#" class="introduce">
                  <div class="flex-column-1 ">
                    <img src="@/assets/img/event-3.jpeg" alt="img-3">
                  </div>
                  <div class="flex-column-2-red">

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
                    <img src="@/assets/img/event-1.jpeg" alt="img-1">
                  </div>
                  <div class="flex-column-2-red">

                  </div>
                </a>
              </div>
              <div class="col-lg-4 col-sm-12 col-12 d-flex flex-column pl-2 pr-2">
                <a href="#" class="introduce">
                  <div class="flex-column-1 ">
                    <img src="@/assets/img/event-2.jpeg" alt="img-2">
                  </div>
                  <div class="flex-column-2-grey">

                  </div>
                </a>
              </div>
              <div class="col-lg-4 col-sm-12 col-12 d-flex flex-column pl-2 pr-2">
                <a href="#" class="introduce">
                  <div class="flex-column-1 ">
                    <img src="@/assets/img/event-3.jpeg" alt="img-3">
                  </div>
                  <div class="flex-column-2-red">

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
                    <img src="@/assets/img/event-1.jpeg" alt="img-1">
                  </div>
                  <div class="flex-column-2-red">

                  </div>
                </a>
              </div>
              <div class="col-lg-4 col-sm-12 col-12 d-flex flex-column pl-2 pr-2">
                <a href="#" class="introduce">
                  <div class="flex-column-1 ">
                    <img src="@/assets/img/event-2.jpeg" alt="img-2">
                  </div>
                  <div class="flex-column-2-grey">

                  </div>
                </a>
              </div>
              <div class="col-lg-4 col-sm-12 col-12 d-flex flex-column pl-2 pr-2">
                <a href="#" class="introduce">
                  <div class="flex-column-1 ">
                    <img src="@/assets/img/event-3.jpeg" alt="img-3">
                  </div>
                  <div class="flex-column-2-red">

                  </div>
                </a>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>
<script>
  export default {
    name: 'Slider'
  }

</script>
<style lang="scss" scoped>
  @import "@/scss/abstracts/_variables";
  @import "@/scss/abstracts/_mixins";

  .introduce {
    height: 22.5rem;
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
    height: 18rem;
    width: 100%;
  }

  .flex-column-2-red {
    height: 4.5rem;
    width: 100%;
    align-items: center;
    background-color: #BC2934;
  }

  .flex-column-2-grey {
    height: 4.5rem;
    width: 100%;
    align-items: center;
    background-color: #474E59;
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

  img {
    width: 100%;
    height: 18rem;
  }

</style>
