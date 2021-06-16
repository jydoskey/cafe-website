<template>
  <div class="navbar my-0" :class="{ change_color: scrollPosition > 80 }">
    <div class="container">
      <div class="logo">
        <NuxtLink to="/">
          <img src="../assets/cafe-one-logo.svg" alt="" />
        </NuxtLink>
      </div>
      <div class="links">
        <div class="about mx-2">
          <NuxtLink to="/about" class="nav-link d-inline-block py-2 px-2"
            >About</NuxtLink
          >
        </div>
        <div class="co-working mx-2">
          <NuxtLink to="/co-working" class="nav-link d-inline-block py-2 px-2"
            >Co-Working</NuxtLink
          >
        </div>
        <div class="events mx-2">
          <NuxtLink to="/events" class="nav-link d-inline-block py-2 px-2"
            >Events</NuxtLink
          >
        </div>
        <div class="community mx-2">
          <NuxtLink to="/community" class="nav-link d-inline-block py-2 px-2"
            >Community</NuxtLink
          >
        </div>
        <div class="cafe mx-2">
          <NuxtLink to="/cafe" class="nav-link d-inline-block py-2 px-2"
            >Cafe</NuxtLink
          >
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data: () => ({
    scrollPosition: 0,
  }),
  methods: {
    updateScroll() {
      this.scrollPosition = window.scrollY;
    },
  },
  mounted() {
    window.addEventListener("scroll", this.updateScroll);
  },
};
</script>

<style lang="scss" scoped>
.navbar {
  /* background: #000; */
  position: sticky;
  top: 0;
  z-index: 50000000;

  &.change_color {
    background: #000;
    /* z-index: 100;
	box-shadow: 0px -3px 12px 8px rgba(0, 0, 0, 0.13);
	box-shadow: 0px 5px 5px 1px rgba(0, 0, 0, 0.2); */
  }

  .links {
    display: flex;

    a {
      color: #fff;
      border-bottom: 3px solid transparent;

      &:hover {
        text-decoration: none;
        border-bottom: 3px solid #bc2934;
        transition: 1s ease all;
      }
    }
  }

  .nav-link.nuxt-link-exact-active {
    border-bottom: 3px solid #bc2934;
  }
}
</style>