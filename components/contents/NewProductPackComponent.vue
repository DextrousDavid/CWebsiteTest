<template>
  <div>
    <div class="our-product">
      <div class="cloudenly-headline" style="text-align: center">
        Explore other Cloudenly Products
      </div>
      <div class="w-full sm:flex justify-center tabs-container">
        <div
          class="tabs-control"
          :class="
            currentTab == 1
              ? 'humanaActive'
              : currentTab == 2
              ? 'optimaActive'
              : currentTab == 3
              ? 'quantumActive'
              : null
          "
        >
          <v-tabs v-model="currentTab" background-color="transparent" grow>
            <!-- <v-tab>Ally</v-tab> -->
            <v-tab>Optima</v-tab>
            <v-tab>HumanaR</v-tab>
            <v-tab>Dome</v-tab>
            <!-- <v-tab>Quantum</v-tab> -->
          </v-tabs>
        </div>

        <v-tabs-items v-model="currentTab">
          <!-- <v-tab-item>
            <div></div>
          </v-tab-item> -->
          <v-tab-item>
            <img
              class="mana-img"
              src="/img/optima-transactions.jpg"
              alt="Optima banner image"
            />
          </v-tab-item>
          <v-tab-item>
            <p>(available shortly...)</p>
          </v-tab-item>
          <v-tab-item>
            <p>(available shortly...)</p>
          </v-tab-item>
          <!-- <v-tab-item>
            <NewProducts :features="quantum_content" />
          </v-tab-item> -->
        </v-tabs-items>
      </div>
    </div>
  </div>
</template>
<script>
// import { VTabs, VTab, VTabItem, VTabsItems } from 'vuetify/lib'
// import NewProducts from './NewProducts'
export default {
  data() {
    return {
      currentTab: 0,
    }
  },
}
</script>
<style scoped>
.mana-img {
  width: 90%;
  image-rendering: -webkit-optimize-contrast;
  margin-top: 2rem;
  margin-left: auto;
  margin-right: auto;
  /* width: 636px;
  height: 420px; */
}
.our-product {
  background: #ffffff;
  padding: 100px 68px;
}

.tabs-container {
  margin-top: 20px;
  flex-direction: column;
  align-items: center;
}
.tabs-control {
}
@media (max-width: 768px) {
  .our-product {
    padding: 0px 0px;
  }
}
</style>
<style>
.tabs-control .v-tab {
  font-size: 16px;
  line-height: 19px;
  font-family: GalanoGrotesque-SemiBold;
}

.tabs-control .v-tabs-slider-wrapper .v-tabs-slider {
  background-color: unset;
}
.tabs-control .v-tab.v-tab--active {
  font-family: GalanoGrotesque-SemiBold;
  font-size: 16px;
  line-height: 19px;
  color: #f1f5fb;
  background: #4781dc;
  border-radius: 3px;
}
.quantumActive .v-tab.v-tab--active {
  background: #525252 !important;
}
.humanaActive .v-tab.v-tab--active {
  background: #5e227f !important;
}
.optimaActive .v-tab.v-tab--active {
  background: #16b271 !important;
}

.v-tabs:not(.v-tabs--vertical) .v-tab {
  white-space: normal;
  margin-left: 35px;
}
/* dome: #05613a green
optima: ##4781dc blue
humanaR: #5e227f purple */
</style>
