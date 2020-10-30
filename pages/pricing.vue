<template>
  <no-ssr>
    <div>
      <AppHeader />
      <v-app>
        <section class="banner">
          <div class="content-center mr-3 ml-3">
            <h1 class="banner-h1 font-bold">Cloudenly Pricing</h1>
            <div style="max-width: 550px; margin: auto">
              <p class="banner-p font-normal">
                Flexible pricing options, from personal projects to enterprise
                applications, and everything in between
              </p>
            </div>
          </div>
        </section>
        <PricingTabs />
        <v-container>
          <div class="mt-16">
            <h3 class="mb-4">Choose the number of users</h3>
            <div>
              <v-btn outlined medium class="d-inline">
                10
                <v-icon right>$expand</v-icon>
              </v-btn>
              <v-btn class="d-inline text-capitalize" color="primary"
                >Users</v-btn
              ><span class="ml-3">N80/user/ Month</span>
            </div>
          </div>
          <!-- Choose your apps starts here -->
          <div>
            <ChooseYourApps />
          </div>
        </v-container>
      </v-app>
    </div>
  </no-ssr>
</template>

<script>
import AppHeader from './../components/header/AppHeader'
import PricingTabs from './../components/contents/PricingTabs'
import ChooseYourApps from './../components/contents/ChooseYourApps'
export default {
  components: {
    AppHeader,
    PricingTabs,
    ChooseYourApps,
  },
  data: () => ({
    currentItem: 'tab-Web',
    items: ['Web', 'Shopping', 'Videos', 'Images'],
    more: ['News', 'Maps', 'Books', 'Flights', 'Apps'],
  }),

  head() {
    return {
      title: 'Cloudenly - Pricing',
      meta: [
        {
          hid: 'Cloudenly - Pricing',
          name: 'Cloudenly - Pricing',
          content:
            'Cloudenly - Flexible pricing options, from personal projects to enterprise applications, and everything in between',
        },
      ],
    }
  },
}
</script>
<style scoped>
* {
  font-family: GalanoGrotesque-Medium;
  /* color: #828282; */
}

h1 {
  line-height: 26px;
  font-size: 22px;
  font-weight: 500;
  margin-top: -50px;
}

p {
  margin-top: 70px;
}

.banner-h1 {
  margin-top: -50px;
  margin-bottom: 10px;
  padding: 10px 0;
  font-size: 36px;
  vertical-align: top;
  color: #fff;
}

.banner-p {
  font-size: 17px;
  text-align: center;
  margin: auto;
  color: #fff;
}

.banner {
  max-width: 100%;
  padding: 11rem 0 9rem 0;
  margin-top: 5rem;
  text-align: center;
  background-image: url('rectangle-banner.png');
  background-repeat: no-repeat;
  background-size: 100% 100%;
  color: white;
}

@media (max-width: 728px) {
  .banner-p {
    font-size: 16px;
  }

  .banner-h1 {
    font-size: 28px;
  }

  .banner {
    background-image: linear-gradient(
      268.51deg,
      #856fee 34.21%,
      #b894f6 73.36%
    );
  }
}
/* .v-application--wrap {
  min-height: 1px !important;
} */

/* @media (max-width: 480px) {
}
@media (max-width: 768px) {
}

@media (max-width: 1024px) {
}
@media (min-width: 1200px) {
} */
</style>
