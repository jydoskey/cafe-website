<template>
  <div class="host-webinar">
    <div class="container host-webinar-body col">
      <div class="d-flex justify-content-center pb-4 text-center">
        <h2 class="newsletter">Host A Webinar</h2>
      </div>
      <div>
        <form class="col-lg-4 col-md-6 justify-content-center mr-auto ml-auto">
          <div class="form-group">
            <input type="text" name="location" class="form-control form-control-lg" id="location"
              aria-describedby="location" placeholder="Location" required />
          </div>
          <div class="form-group">
            <input type="text" name="meeting-room" class="form-control form-control-lg" id="meeting-room"
              aria-describedby="meeting-room" placeholder="Meeting Room" required />
          </div>
          <div class="form-group">
            <input type="number" name="peopleNum" class="form-control form-control-lg" id="peopleNum"
              aria-describedby="peopleNum" placeholder="Number of People" required />
          </div>
          <div class="form-group">
            <input type="date" name="date" class="form-control form-control-lg" id="date" aria-describedby="date"
              placeholder="Date" required />
          </div>
          <div class="text-center">
            <button type="submit" id="submit" name="submit" class="btn btn-lg btn-block btn-red">
              BOOK
            </button>
          </div>
        </form>
      </div>
    </div>
  </div>
</template>
<script>
  export default {
    name: "host-webinar",
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
    background: #FFE6BA !important;
    border: 0px !important;
    border-radius: 0% !important;
  }

  ::placeholder {
    font-size: 16px;
  }

  .btn-red {
    border-radius: 0% !important;
    font-size: 16px;
    height: 3.5rem;
  }

  .host-webinar {
    background-color: #FFD68F;
    margin: 10px 0px 80px;
    color: #474E59;
    padding-bottom: 2rem;
  }

  .host-webinar-body {
    width: 1150px;
    margin: auto;
    padding-top: 50px;
    padding-bottom: 20px;
  }

  .host-webinar-body h2 {
    font-weight: 800;
    font-stretch: normal;
    font-style: normal;
    letter-spacing: normal;
    color: #474E59;
  }

  span {
    margin: 10px;
  }

  @media only screen and (max-width: 1150px) {
    .host-webinar-body {
      display: block;
      align-items: center;
      justify-content: center;
    }

    .host-webinar-body h2 {
      font-size: 32px;
    }

  }

  @media only screen and (max-width: 1150px) {
    .host-webinar-body {
      width: 99%;
    }
  }

  .newsletter {
    font-size: 2.125rem;
    line-height: 44px;
  }

  input::-webkit-datetime-edit,
  input::-webkit-inner-spin-button,
  input::-webkit-clear-button {
    font-size: 16px;
    color: gray;
  }

</style>
