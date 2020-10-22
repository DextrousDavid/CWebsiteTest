<template>
  <div>
    <v-tabs
      fixed-tabs
      height="60"
      centered
      right
      light
      center-active
      background-color="grey lighten-3"
    >
      <v-tab>Guided <v-icon right>$expand</v-icon></v-tab>
      <v-tab><img src="~assets/tabIcons/lite.png" /> Lite</v-tab>
      <v-tab><img src="~assets/tabIcons/optima.png" />Optima</v-tab>
      <v-tab><img src="~assets/tabIcons/humanaR.png" />HumanaR</v-tab>
      <v-tab><img src="~assets/tabIcons/dome.png" />Dome</v-tab>
      <v-tab><img src="~assets/tabIcons/ally.png" />Ally</v-tab>
      <v-tab><img src="~assets/tabIcons/quantum.png" />Quantum</v-tab>
      <v-tab style="background-color: #fff; color: #000">
        <p style="font-size: 9px">
          No of products: 3<br /><span class="total-no">
            Total No of Apps: 12</span
          >
        </p></v-tab
      >
      <v-tab style="background-color: #1976d2; color: #fff">
        <p class="float-left" style="font-size: 8px">50, 000 per Month</p>

        <v-btn class="float-right" x-small elevation="2">Buy Now</v-btn>
      </v-tab>
    </v-tabs>
  </div>
</template>

<script>
export default {
  name: 'PricingTabs',
}
</script>

<style scoped>
.total-no {
  font-weight: 900;
}
.exact-active-class {
  color: red;
}
* {
  font-family: GalanoGrotesque-Medium;
  /* color: #828282; */
}
.v-tab {
  align-items: center;
  display: flex;
  flex: 0 1 auto;
  font-size: 0.875rem;
  font-weight: 500;
  justify-content: center;
  letter-spacing: 0.0892857143em;
  line-height: normal;
  min-width: 90px;
  max-width: 360px;
  outline: none;
  padding: 0 16px;
  position: relative;
  text-align: center;
  text-decoration: none;
  text-transform: capitalize;
  transition: none;

  -webkit-user-select: none;
  -moz-user-select: none;
  -ms-user-select: none;
  user-select: none;
}

img {
  margin-right: 5px;
}
</style>
