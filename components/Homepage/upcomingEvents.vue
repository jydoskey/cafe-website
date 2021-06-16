<template>
  <div class="upcomingevents">
    <div class="container upcomingevents-body col justify-content-between">
      <div>
        <span class="events">UPCOMING EVENTS &nbsp;<img src="@/assets/img/events-marker.svg" alt="event marker"></span>
        <h2>Café One Talk And<br /> Events</h2>
      </div>
      <span class="upcomingevents-text d-flex justify-content-between align-items-center">
        Some text about events come here. Some text<br /> about events come here
        <nuxt-link to="/events">
          <span class="link-text">View all events &nbsp;&nbsp;<img src="@/assets/img/more-events-arrow.svg"
              alt="more events arrow"></span>
        </nuxt-link>
      </span>
      <div class="tables text-start">
        <slider />
      </div>
    </div>
  </div>
</template>
<script>
  import slider from "@/components/slider.vue";
  export default {
    name: "upcomingEvents",
    data() {
      return {}
    },
    components: {
      slider
    }
  };

</script>
<style lang="scss" scoped>
  @import "@/scss/abstracts/_variables";
  @import "@/scss/abstracts/_mixins";

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
    font-family: Lato;
  }

  .upcomingevents {
    margin: 40px 0px 0;
  }

  .upcomingevents-body {
    width: 1150px;
    margin: auto;
    padding-top: 50px;
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

  a:link {
    text-decoration: none;
  }

  .link-text {
    color: #BC2934
  }

  .link-text:hover {
    color: #d11d2b;
  }

</style>
