<template>
  <div class="upcomingevents">
    <div class="container upcomingevents-body col justify-content-between">
      <div>
        <span class="events">UPCOMING EVENTS &nbsp;<img src="@/assets/img/events-marker.svg" alt="event marker"></span>
        <h2>Some Text About Events That<br /> Will Happen</h2>
      </div>
      <div class="tables text-start pt-5">
        <div class="container col pb-5 position-relative pr-0 pl-0">
          <div class="carousel position-relative" data-ride="carousel">
            <!-- The slideshow -->
            <div class="carousel-inner">
              <div class="carousel-item carousel-item-next carousel-item-left">
                <div class="d-flex justify-content-between">
                  <div class="col-lg-4 col-sm-12 col-12 d-flex flex-column pl-2 pr-2">
                    <a href="#" class="introduce">
                      <div class="flex-column-1 ">
                        <img src="@/assets/img/upcoming-1.jpeg" alt="img-1">
                      </div>
                      <div class="d-flex flex-column-2-grey align-items-center">
                        <div class="event-time p-2">
                          <span>10 April</span>
                          <span>9am - 10am</span>
                        </div>
                        <div class="register text-center">
                          Register &nbsp;&nbsp;<img src="@/assets/img/register.png" alt="register">
                        </div>
                      </div>
                    </a>
                  </div>
                  <div class="col-lg-4 col-sm-12 col-12 d-flex flex-column pl-2 pr-2">
                    <a href="#" class="introduce">
                      <div class="flex-column-1 ">
                        <img src="@/assets/img/upcoming-2.jpeg" alt="img-2">
                      </div>
                      <div class="d-flex flex-column-2-grey align-items-center">
                        <div class="event-time p-2">
                          <span>10 April</span>
                          <span>9am - 10am</span>
                        </div>
                        <div class="register text-center">
                          Register &nbsp;&nbsp;<img src="@/assets/img/register.png" alt="register">
                        </div>
                      </div>
                    </a>
                  </div>
                  <div class="col-lg-4 col-sm-12 col-12 d-flex flex-column pl-2 pr-2">
                    <a href="#" class="introduce">
                      <div class="flex-column-1 ">
                        <img src="@/assets/img/upcoming-3.jpeg" alt="img-3">
                      </div>
                      <div class="d-flex flex-column-2-grey align-items-center">
                        <div class="event-time p-2">
                          <span>10 April</span>
                          <span>9am - 10am</span>
                        </div>
                        <div class="register text-center">
                          Register &nbsp;&nbsp;<img src="@/assets/img/register.png" alt="register">
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
    name: "upcomingEvents",
    data() {
      return {}
    },

  };

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

  .flex-column-1 img {
    width: 100%;
    height: 18rem;
  }

  .upcomingevents-text {
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

  .upcomingevents {
    margin: 0px 0px 0;
  }

  .upcomingevents-body {
    width: 1150px;
    margin: auto;
    padding-top: 10px;
    padding-bottom: 20px;
  }

  .upcomingevents-body h2 {
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

  .bitmap {
    max-width: 1100px;
    width: 100%;
    height: auto;
    margin: 0;
    object-fit: contain;
  }

  span {
    margin: 10px;
  }

  @media only screen and (max-width: 1150px) {
    .upcomingevents-body {
      display: block;
      align-items: center;
      justify-content: center;
    }

    .upcomingevents-body h2 {
      font-size: 32px;
    }

    .upcomingevents-body p {
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
    .upcomingevents-body {
      width: 99%;
    }

    .upcomingevents-body p {
      margin-bottom: 30px;
    }
  }

  .events {
    font-style: normal;
    font-weight: 500;
    font-size: 20px;
    line-height: 30px;
    color: #222831;
    margin: 0;
    font-family: Lato;
  }


  .event-time span {
    font-family: Lato;
    font-style: normal;
    font-weight: 500;
    font-size: 16px;
    line-height: 28px;
    color: #FFFFFF;
    display: block;
  }

  .event-time {
    width: 50%;
  }

  .register {
    width: 50%;
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

</style>
