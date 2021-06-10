<template>
  <footer class="cafe-footer">
    <div class="container">
      <div class="row">
        <div class="col-12 col-lg-4 col-md-12">
          <div class="cafe-footer__section footer-header">
            <h6 class="company-footer__heading">Café One</h6>
            <p class="cafe-footer__link">At Café One, innovation meets community.<br /> We play host to Sterling Bank’s
              digital <br /> products; offering
              premium banking services<br /> and the best coffee in Lagos.</p>
            <div class="social-links">
              <a v-for="link in socialLink" :key="link.name" :href="link.url" target="_blank" class="social-link">
                <img class="icon" :src="require('@/assets/img/' + link.iconClass + '')" alt="social-icons">
              </a>
            </div>
          </div>
        </div>
        <div class="col-6 col-lg-2">
          <div class="cafe-footer__section">
            <h6 class="cafe-footer__heading">Spaces</h6>
            <ul class="cafe-footer__links">
              <li v-for="link in spacesLinks" :key="link.name">
                <router-link :to="link.url" class="cafe-footer__link">{{link.name}}</router-link>
              </li>
            </ul>
          </div>
        </div>

        <div class="col-6 col-lg-2">
          <div class="cafe-footer__section">
            <h6 class="cafe-footer__heading">Company</h6>
            <ul class="cafe-footer__links">
              <li v-for="link in companyLinks" :key="link.name">
                <router-link :target="link.target" :to="link.url" class="cafe-footer__link">{{link.name}}</router-link>
              </li>
            </ul>
          </div>
        </div>

        <div class="col-6 col-lg-2">
          <div class="cafe-footer__section">
            <h6 class="cafe-footer__heading">Support</h6>
            <ul class="cafe-footer__links">
              <li v-for="link in supportLinks" :key="link.name">
                <a :href="link.url" :target="link.target" class="cafe-footer__link">{{link.name}}</a>
              </li>
            </ul>
          </div>
        </div>

        <div class="col-6 col-lg-2">
          <div class="cafe-footer__section">
            <h6 class="cafe-footer__heading">Contact Us</h6>
            <ul class="cafe-footer__links">
              <li v-for="link in contactLinks" :key="link.name">
                <a :href="link.url" :target="link.target" class="cafe-footer__link">{{link.name}}</a>
              </li>
            </ul>
          </div>
        </div>
      </div>
    </div>
  </footer>
</template>

<script>
  export default {
    name: "Footer",
    data() {
      return {
        companyLinks: [{
            name: 'About Us',
            url: ''
          },
          {
            name: 'Pricing',
            url: '',
            target: '_blank'
          },
          {
            name: 'Careers',
            url: ''
          },
          {
            name: 'Press',
            url: ''
          }
        ],

        spacesLinks: [{
            name: 'Co-working spaces',
            url: '',
            target: '_blank'
          },
          {
            name: 'Meeting rooms',
            url: ''
          },
          {
            name: 'Event spaces',
            url: '',
            target: '_blank'
          },
          {
            name: 'Child playground',
            url: '',
            target: '_blank'
          },
          {
            name: 'Cafe & resto',
            url: '',
            target: '_blank'
          }
        ],

        supportLinks: [{
            name: 'FAQs',
            url: ''
          },
          {
            name: 'Privacy Policy',
            url: ''
          },
          {
            name: 'Help',
            url: '',
            target: '_blank'
          }
        ],

        contactLinks: [{
            name: 'cafe.one@sterling.ng',
            url: 'mailto:cafe.one@sterling.ng'
          },
          {
            name: 'Admiralty Way, Lekki Phase I, Lagos',
            url: 'https://goo.gl/maps/vU162xSLvpZ6WVqC9',
            target: '_blank'
          },
          {
            name: '+2349053872953',
            url: 'tel:+2349053872953'
          }
        ],

        socialLink: [{
            name: 'facebook',
            url: '',
            iconClass: 'facebook.svg'
          },
          {
            name: 'twitter',
            url: '',
            iconClass: 'twitter.svg'
          },
          {
            name: 'instagram',
            url: '',
            iconClass: 'instagram.svg'
          },
        ],
      }
    },
  }

</script>

<style scoped lang="scss">
  @import "@/scss/abstracts/_variables";
  @import "@/scss/abstracts/_mixins";

  .cafe-footer {
    position: relative;
    padding-top: 2.5rem;
    background: black;

    @include breakpoint-min (lg) {
      padding-top: 2.25rem;
    }
  }

  .cafe-footer__section {
    margin-bottom: 2.5rem;
  }

  .cafe-footer__heading {
    margin-bottom: 1rem;
    font-size: 1rem;
    font-weight: bold;
    line-height: 1.25rem;
    color: white;
    opacity: 0.5;

    @include breakpoint-min(lg) {
      margin-bottom: 1.5rem;
      font-size: 1.25rem;
      line-height: 1.5rem;
    }
  }

  .cafe-footer__links {
    margin: 0;
    padding: 0;
    list-style: none;
  }

  .cafe-footer__link {
    display: inline-block;
    margin-bottom: .75rem;
    font-size: .875rem;
    line-height: 1.25rem;
    color: white;
    text-decoration: none;
    transition: .3s ease all;

    @include breakpoint-min(lg) {
      margin-bottom: 1rem;
      font-size: 1rem;
      line-height: 1.5rem;
    }

    &[href]:hover,
    &:focus {
      color: red;
    }

    &.cafe-footer__link--primary {
      color: red;
    }
  }

  .social-links {
    display: flex;
    margin-bottom: 2.5rem;

    @include breakpoint-max (lg) {
      margin: 0 auto;
      justify-content: center;
    }
  }

  .social-link {
    display: block;
    font-size: 1.5rem;
    line-height: 1;
    text-decoration: none;
    color: black;
    margin-right: 2rem;

    &:last-child {
      margin-right: 0;
    }

    i {
      display: block;
    }

    &:hover,
    &:focus {
      color: $red;
    }
  }

  .footer-logo {
    height: 1.5rem;
    width: auto;
  }

  .footer-playstore {
    border-bottom: 1px solid #EBEAED;
    padding: 2.25rem 0;
  }

  .company-footer__heading {
    font-family: Lora;
    font-style: normal;
    font-weight: bold;
    font-size: 52px;
    line-height: 67px;
    color: #FFFFFF;
  }

  .icon {
    width: 2rem;
    height: 2rem;
  }

  .footer-header {
    @include breakpoint-max (lg) {
      text-align: center;
    }
  }

</style>
