<template>
  <div class="navbar p-0 m-0" :class="{ change_color: scrollPosition > 94 }">
    <div class="container">
      <div class="logo">
        <NuxtLink to="/">
          <img src="@/assets/cafe-one-logo.svg" alt="" />
        </NuxtLink>
      </div>
      <div class="links d-none d-lg-flex">
        <div class="about mx-2">
          <NuxtLink to="/#about-section" class="nav-link d-inline-block py-2 px-2">About</NuxtLink>
        </div>
        <div class="co-working mx-2">
          <NuxtLink to="/co-work" class="nav-link d-inline-block py-2 px-2">Co-Working</NuxtLink>
        </div>
        <div class="events mx-2">
          <NuxtLink to="/events" class="nav-link d-inline-block py-2 px-2">Events</NuxtLink>
        </div>
        <div class="community mx-2">
          <NuxtLink to="/community" class="nav-link d-inline-block py-2 px-2">Community</NuxtLink>
        </div>
        <div class="cafe mx-2">
          <NuxtLink to="/cafe" class="nav-link d-inline-block py-2 px-2">Cafe</NuxtLink>
        </div>
      </div>

      <div @click="toggleMobileNav" class="mobile-nav d-block d-lg-none">
        <p>Menu&nbsp;<img src="@/assets/img/hamburger.svg" alt="hamburger=menu"></p>
      </div>
    </div>

    <div class="mobileNav" v-if="isNavShown">
      <div class="header d-flex px-3" @click="isNavShown = false">
        <p class="d-inline-block m-0 p-2 mr-3">Close</p>
      </div>
      <div class="linkss">
        <div class="about mx-2" @click="closeMobileNav">
          <NuxtLink to="/#about" class="nav-link d-inline-block py-2 px-2" @click="isNavShown = false">About</NuxtLink>
        </div>
        <div class="co-working mx-2" @click="closeMobileNav">
          <NuxtLink to="/co-work" class="nav-link d-inline-block py-2 px-2" @click="isNavShown = false">Co-Working
          </NuxtLink>
        </div>
        <div class="events mx-2" @click="closeMobileNav">
          <NuxtLink to="/events" class="nav-link d-inline-block py-2 px-2" @click="isNavShown = false">Events</NuxtLink>
        </div>
        <div class="community mx-2" @click="closeMobileNav">
          <NuxtLink to="/community" class="nav-link d-inline-block py-2 px-2" @click="isNavShown = false">Community
          </NuxtLink>
        </div>
        <div class="cafe mx-2" @click="closeMobileNav">
          <NuxtLink to="/cafe" class="nav-link d-inline-block py-2 px-2">Cafe</NuxtLink>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
  export default {
    data: () => ({
      scrollPosition: 0,
      isNavShown: false,
    }),
    methods: {
      updateScroll() {
        this.scrollPosition = window.scrollY;
      },
      toggleMobileNav() {
        this.isNavShown = !this.isNavShown;
      },
      closeMobileNav() {
        this.isNavShown = false;
      },
    },
    mounted() {
      window.addEventListener("scroll", this.updateScroll);
    },
  };

</script>

<style lang="scss" scoped>
  .navbar {
    background: rgba(0, 0, 0, 0.5);
    position: absolute;
    top: 0;
    width: 100%;
    z-index: 50000000;

    &.change_color {
      background: #000;
      position: sticky;
    }

    .links {
      display: flex;

      a {
        color: #fff;
        border-bottom: 3px solid transparent;
        cursor: pointer;

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

    .mobile-nav {
      p {
        color: #fff;
        margin: 0;
        padding: 0;
        padding: 8px;
        cursor: pointer;
      }
    }

    .mobileNav {
      position: absolute;
      top: 0;
      bottom: 0;
      height: 100vh;
      width: 100vw;
      z-index: 1000000000000;
      background: #ffe6ba;

      .header {
        height: 60px;
        display: flex;
        justify-content: flex-end;
        align-items: center;
        border-bottom: 2px solid maroon;

        p {
          cursor: pointer;
          color: #bc2934;
        }
      }

      .linkss {
        height: calc(100% - 60px);
        background: #bc2934;
        width: 100%;
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;

        a {
          color: #ffe6ba;
          border-bottom: 3px solid #bc2934;
          cursor: pointer;

          &:hover {
            text-decoration: none;
            border-bottom: 3px solid #ffe6ba;
            transition: 1s ease all;
          }
        }
      }
    }
  }

</style>
