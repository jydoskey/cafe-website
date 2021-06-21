<template>
  <div class="communities">
    <section class="container">
      <div class="home-section home-section-b">
        <div>
          <span class="our-communities">OUR COMMUNITIES &nbsp;<img src="@/assets/img/events-marker.svg"
              alt="event marker"></span>
          <h2>Some General Info About<br /> Café One Communities</h2>
        </div>
        <div class="row">
          <div class="col-md-12">
            <div class="community align-items-center justify-content-center">
              <div class="col-lg-4 pt-3 com-col"><img class="community-img" src="@/assets/img/creatives.jpeg"
                  alt="creatives-svg"></div>
              <div class="community-text col-lg-5">
                <h6 class="community-h6">
                  Creatives
                </h6>
                <p class="community-p">
                  Nulla porttitor accumsan tincidunt. Curabitur aliquet quam id dui posuere blandit. Curabitur aliquet
                  quam id dui posuere blandit. Curabitur arcu erat, accumsan id imperdiet et, porttitor at sem.
                </p>
                <div class="text-center pt-2">
                  <button type="submit" id="submit" name="submit" class="col-5 btn btn-lg btn-block btn-red">
                    JOIN
                  </button>
                </div>
              </div>
            </div>

            <div class="community-reverse align-items-center justify-content-center">
              <div class="community-text col-lg-5">
                <h6 class="community-h6">
                  Food Club
                </h6>
                <p class="community-p">
                  Nulla porttitor accumsan tincidunt. Curabitur aliquet quam id dui posuere blandit. Curabitur aliquet
                  quam id dui posuere blandit. Curabitur arcu erat, accumsan id imperdiet et, porttitor at sem.
                </p>
                <div class="text-center pt-2">
                  <button type="submit" id="submit" name="submit" class="col-5 btn btn-lg btn-block btn-red">
                    JOIN
                  </button>
                </div>
              </div>
              <div class="col-lg-4 pt-3 com-rev-col">
                <img class="community-img" src="@/assets/img/food.jpeg" alt="food-club-svg">
              </div>
            </div>

            <div class="community align-items-center justify-content-center">
              <div class="col-lg-4 pt-3 com-col">
                <img class="community-img" src="@/assets/img/yoga.jpeg" alt="fitness-svg">
              </div>
              <div class="community-text col-lg-5">
                <h6 class="community-h6">Fitness and Wellbeing</h6>
                <p class="community-p">
                  Nulla porttitor accumsan tincidunt. Curabitur aliquet quam id dui posuere blandit. Curabitur aliquet
                  quam id dui posuere blandit. Curabitur arcu erat, accumsan id imperdiet et, porttitor at sem.
                </p>
                <div class="text-center pt-2">
                  <button type="submit" id="submit" name="submit" class="col-5 btn btn-lg btn-block btn-red">
                    JOIN
                  </button>
                </div>
              </div>
            </div>

            <div class="community-reverse align-items-center justify-content-center">
              <div class="community-text col-lg-5">
                <h6 class="community-h6">New Moms</h6>
                <p class="community-p">
                  Nulla porttitor accumsan tincidunt. Curabitur aliquet quam id dui posuere blandit. Curabitur aliquet
                  quam id dui posuere blandit. Curabitur arcu erat, accumsan id imperdiet et, porttitor at sem.
                </p>
                <div class="text-center pt-2">
                  <button type="submit" id="submit" name="submit" class="col-5 btn btn-lg btn-block btn-red">
                    JOIN
                  </button>
                </div>
              </div>
              <div class="col-lg-4 pt-3 com-rev-col">
                <img class="community-img" src="@/assets/img/mom-community.png" alt="new-moms-svg">
              </div>
            </div>
          </div>
        </div>
      </div>
    </section>
  </div>
</template>
<script>
  export default {
    name: "ourCommunities",
  };

</script>


<style lang='scss' scoped>
  @import "@/scss/abstracts/_variables";
  @import "@/scss/abstracts/_mixins";

  .community {
    display: flex;
    flex-direction: column;
    padding-top: 5rem;

    @include breakpoint-min(sm) {
      max-width: unset;
    }

    @include breakpoint-min(md) {
      flex-direction: row;
      align-items: center;
    }

  }

  .home-section h2 {
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

  @media only screen and (max-width: 1150px) {
    .our-communities {
      font-style: normal;
      font-weight: 500;
      font-size: 20px;
      line-height: 30px;
      margin: 0;
      font-family: Lato;
      color: #474E59;
    }
  }

  .community-reverse {
    display: flex;
    flex-direction: column-reverse;
    padding-top: 5rem;

    @include breakpoint-min(sm) {
      max-width: unset;
    }

    @include breakpoint-min(md) {
      flex-direction: row;
      align-items: center;
    }
  }

  .communities {
    background-color: #FFF5E4;
    padding-bottom: 10rem;
    padding-top: 4rem;
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

    @media (min-width:1400px) {
      max-width: 1300px;
    }
  }

  .row {
    @media (min-width: 320px) {
      flex-direction: column-reverse;
    }

    @media (min-width: 992px) {
      flex-direction: row;
    }

    @media (min-width: 1200px) {
      flex-direction: row;
      margin-left: -15px;
    }
  }

  .row-1 {
    padding-bottom: 20px;
  }

  .community-text {
    p {
      font-size: 1rem;
      font-weight: bold;
    }
  }

  @media (max-width: 991px) {
    .community-text {
      grid-row: 1/3;
    }
  }

  .home-section {
    @media (min-width: 280px) {
      padding: 0;
    }

    @include breakpoint-min(lg) {
      padding-bottom: 5rem;
    }

    @media (min-width:1500px) {
      padding-bottom: 6rem;
    }
  }



  .home-section-b {
    padding-bottom: 0;
  }

  .community-h6 {
    color: #6A6A6A;
    font-family: Lora;
    font-style: normal;
    font-weight: bold;
    line-height: 41px;

    @media (min-width: 280px) {
      font-size: 1.125rem;
    }

    @include breakpoint-min(md) {
      font-size: 1.125rem;
    }

    @include breakpoint-min(lg) {
      font-size: 1.5625rem;
    }

    @include breakpoint-min(xl) {
      font-size: 1.875rem;
    }
  }

  .community-p {
    font-family: Lato;
    font-style: normal;
    font-weight: 500;
    font-size: 18px;
    line-height: 28px;
    color: #6A6A6A;

    @media (min-width: 280px) {
      font-size: 0.75rem;
    }

    @include breakpoint-min(md) {
      font-size: 0.875rem;
    }

    @include breakpoint-min(lg) {
      font-size: 1rem;
      max-width: 90%;
    }

    @include breakpoint-min(xl) {
      font-size: 1.125rem;
      max-width: 100%;
    }
  }

  .p-style {
    color: #303030;

    @media (min-width: 280px) {
      font-size: 0.75rem;
    }

    @media (min-width: 425px) {
      font-size: 1rem;
    }

    @media (min-width: 576px) {
      font-size: 1.125rem;
    }

    @media (min-width: 1200px) {
      margin-bottom: 0.625rem;
    }
  }

  .btn-red {
    border-radius: 0% !important;
    font-size: 16px;
    height: 3.5rem;
  }

  .community-img {
    width: 280px;
    height: 280px;
    z-index: 999;
  }

  .com-col {
    position: relative;
    z-index: 1;

    &::after {
      content: "";
      position: absolute;
      left: 0rem;
      top: 3rem;
      width: 280px;
      height: 280px;
      z-index: -1;
      background: rgba(196, 196, 196, 0.27);
    }

    @include breakpoint-max (md) {
      &::after {
        content: "";
        background: #FFF5E4;
      }
    }
  }

  .com-rev-col {
    position: relative;
    z-index: 1;

    &::after {
      content: "";
      position: absolute;
      left: 1.8rem;
      top: 3rem;
      width: 280px;
      height: 280px;
      z-index: -1;
      background: rgba(196, 196, 196, 0.27);
    }

    @include breakpoint-max (md) {
      &::after {
        content: "";
        background: #FFF5E4;
      }
    }
  }

</style>
