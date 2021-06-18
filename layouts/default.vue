<template>
  <div>
    <navBar />
    <Nuxt />
    <app-footer />
  </div>
</template>

<script>
  import appFooter from "@/layouts/appFooter.vue";
  import navBar from "@/layouts/navBar.vue";
  export default {
    components: {
      appFooter,
      navBar,
    },
  };

</script>

<style lang="scss">
  @import "@/scss/vendor/themed-bootstrap.scss";
  @import "@/scss/main.scss";

  body {
    overflow-x: hidden !important;
  }

  .text-red {
    color: #BC2934;
  }

  .app-body {
    display: flex;
    flex-direction: column;
    flex-wrap: nowrap;
    min-height: 100vh;
    margin: 0 auto;
  }

  .app-main {
    flex: 1 0 auto;
  }

  .btn {
    border-radius: 10px;
  }

  .btn-green {
    background-color: #29b36a;
    color: #fff;
  }

  .btn-red {
    background-color: #bc2934;
    color: #fff;
  }

  .no-gap {
    padding-right: 0;
    padding-left: 0;
  }

  .top-page {
    margin-top: 78px;

    @include breakpoint-min(md) {
      margin-top: 78px;
    }
  }

</style>
