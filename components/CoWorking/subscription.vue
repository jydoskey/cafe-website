<template>
  <div class="subscription">
    <div class="container subscription-body col justify-content-between">
      <div>
        <span class="cafe-subscription"
          >SUBSCRIBE &nbsp;<img
            src="@/assets/img/events-marker.svg"
            alt="subscription marker"
        /></span>
        <h2>Our subscription plans</h2>
      </div>
      <div class="tables text-start">
        <div class="container col pt-5 position-relative pr-0 pl-0">
          <div class="card-deck">
            <div class="card text-center">
              <div class="card-body">
                <h5 class="card-title">Weekly Plan</h5>
                <p class="card-text">
                  Nulla porttitor accumsan tincidunt. Curabitur aliquet quam id
                  dui posuere blandit.
                </p>
                <p class="card-pricing">N 20,000</p>
              </div>
              <div class="card-footer pt-3 pb-3">PAY NOW</div>
            </div>
            <div class="card text-center">
              <div class="card-body">
                <h5 class="card-title">Monthly Plan</h5>
                <p class="card-text">
                  Nulla porttitor accumsan tincidunt. Curabitur aliquet quam id
                  dui posuere blandit.
                </p>
                <p class="card-pricing">N 40,000</p>
              </div>
              <div class="card-footer pt-3 pb-3">PAY NOW</div>
            </div>
            <div class="card text-center">
              <div class="card-body">
                <h5 class="card-title">Yearly Plan</h5>
                <p class="card-text">
                  Nulla porttitor accumsan tincidunt. Curabitur aliquet quam id
                  dui posuere blandit.
                </p>
                <p class="card-pricing">N 50,000</p>
              </div>
              <div class="card-footer pt-3 pb-3">PAY NOW</div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  name: "subscription",
  data() {
    return {};
  },
};
</script>
<style lang="scss" scoped>
@import "@/scss/abstracts/_variables";
@import "@/scss/abstracts/_mixins";

.subscription {
  margin: 40px 0px 50px;
}

.subscription-body {
  width: 1150px;
  margin: auto;
  padding-top: 50px;
  padding-bottom: 20px;
}

.subscription-body h2 {
  font-size: 40px;
  font-weight: 800;
  font-stretch: normal;
  font-style: normal;
  line-height: 1.18;
  letter-spacing: normal;
  color: #474e59;
  text-align: start;
  font-family: Lora;
}

.tables {
  border-radius: 2px;
  margin-bottom: 20px;
}

span {
  margin: 10px;
}

@media only screen and (max-width: 1150px) {
  .subscription-body {
    display: block;
    align-items: center;
    justify-content: center;
  }

  .subscription-body h2 {
    font-size: 32px;
  }

  .subscription-body p {
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
  .subscription-body {
    width: 99%;
  }

  .subscription-body p {
    margin-bottom: 30px;
  }
}

.cafe-subscription {
  font-style: normal;
  font-weight: 500;
  font-size: 20px;
  line-height: 30px;
  color: #222831;
  margin: 0;
  text-transform: uppercase;
  font-family: Lato;
}

.card-footer {
  background-color: #bc2934;
  color: white;
  border-radius: 0;
}

.card-title {
  font-family: Lora;
  font-style: normal;
  font-weight: normal;
  font-size: 26px;
  line-height: 33px;
  color: #303030;
  padding-top: 1.5rem;
}

.card-text {
  font-family: Lato;
  font-style: normal;
  font-weight: 300;
  font-size: 18px;
  line-height: 28px;
  color: #9a9a9a;
  padding-top: 1rem;
}

.card-pricing {
  font-family: Lora;
  font-style: normal;
  font-weight: bold;
  font-size: 26px;
  line-height: 33px;
  color: #474e59;
  padding-top: 1.5rem;
  padding-bottom: 1.5rem;
}
</style>
