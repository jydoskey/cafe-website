<template>
  <div class="cafe-locations">
    <div class="container cafe-locations-body col">
      <div class="d-flex justify-content-center pb-2">
        <h2 class="locations">Café One L<img src="@/assets/img/location-marker.svg" alt="location-marker">cations</h2>
      </div>
      <div class="tables text-center pb-5">
        <iframe
          src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d3964.6479412235403!2d3.4533467144402255!3d6.439238795341319!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x103bf5e96eb18d0f%3A0xea70f249cc20b528!2sCaf%C3%A9%20One%20by%20Sterling!5e0!3m2!1sen!2sng!4v1623297643972!5m2!1sen!2sng"
          class="bitmap" style="border:0;" allowfullscreen="" loading="lazy"></iframe>
      </div>
      <div class="d-flex justify-content-center pb-4 text-center">
        <h2 class="newsletter">Subscribe To Our Newsletters</h2>
      </div>
      <div>
        <form class="col-lg-4 justify-content-center mr-auto ml-auto">
          <div class="form-group">
            <input type="email" name="email" class="form-control form-control-lg email" id="email"
              aria-describedby="email" placeholder="Email" />
          </div>
          <div class="text-center">
            <button type="submit" id="submit" name="submit" class="btn btn-lg btn-block btn-red">
              SUBSCRIBE
            </button>
          </div>
        </form>
      </div>
    </div>
  </div>
</template>
<script>
  export default {
    name: "cafe-locations",
    data() {
      return {}
    },
  };

</script>
<style lang="scss" scoped>
  @import "@/scss/abstracts/_variables";
  @import "@/scss/abstracts/_mixins";

  input {
    height: 4.25rem !important;
    background: transparent !important;
    border: 1px solid #474E59 !important;
    border-radius: 0% !important;
  }

  ::placeholder {
    font-size: 16px;
  }

  .btn-red {
    border-radius: 0% !important;
    font-size: 16px;
    height: 3rem;
  }

  .cafe-locations {
    background-color: #ffffff;
    margin: 80px 0px;
    color: #474E59;
  }

  .cafe-locations-body {
    width: 1150px;
    margin: auto;
    padding-top: 50px;
    padding-bottom: 20px;
  }

  .cafe-locations-body h2 {
    font-weight: 800;
    font-stretch: normal;
    font-style: normal;
    letter-spacing: normal;
    color: #474E59;
  }

  .cafe-locations-body p {
    max-width: 1070px;
    width: 100%;
    height: 64px;
    font-family: Muli;
    font-size: 14px;
    font-weight: 800;
    font-stretch: normal;
    font-style: normal;
    line-height: 1.5;
    letter-spacing: normal;
    color: #1d1f24;
  }

  .tables {
    border-radius: 2px;
    margin-bottom: 20px;
  }

  .bitmap {
    width: 100%;
    height: 25rem;
    margin: 0;
    object-fit: contain;
  }

  span {
    margin: 10px;
  }

  @media only screen and (max-width: 1150px) {
    .cafe-locations-body {
      display: block;
      align-items: center;
      justify-content: center;
    }

    .cafe-locations-body h2 {
      font-size: 32px;
    }

    .cafe-locations-body p {
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
    .cafe-locations-body {
      width: 99%;
    }

    .cafe-locations-body p {
      margin-bottom: 30px;
    }
  }

  .newsletter {
    font-size: 2.125rem;
    line-height: 44px;
  }

  .locations {
    font-size: 2.5rem;
    line-height: 51px;
  }

</style>
