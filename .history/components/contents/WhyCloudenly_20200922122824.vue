<template>
  <div>
    <div class="product-wrapper">
      <div class="why-cloudenly">
        <div class="section-name">Why Cloudenly?</div>
        <div class="w-full sm:flex justify-center tabs-wrapper">
          <div class="section-tabs">
            <v-tabs
              v-model="tab"
              background-color="transparent"
              color="basil"
              grow
            >
              <v-tab v-for="item in items" :key="item">
                {{ item }}
              </v-tab>
            </v-tabs>
          </div>
          <v-tabs-items v-model="tab">
            <v-tab-item>
              <div class="sm:flex" style="margin-top: 56px">
                <div class="sm:w-1/2 sm:flex justify-center sm:mr-4">
                  <div class="section-content">
                    <img src="/img/innovation-icon.svg" />
                    <div class="innovation-text">Innovation</div>
                    <div class="section-text">{{ innovationText }}</div>
                  </div>
                </div>
                <div class="sm:w-1/2 sm:flex justify-center sm:ml-4">
                  <img src="/img/innovation-frame.svg" />
                </div>
              </div>
            </v-tab-item>
            <v-tab-item>
              <div class="md:flex round-card" style="margin-top: 56px">
                <div class="flex-2 card-text-div">
                  <div class="card-header">Scalability</div>
                  <div class="card-inner-text">
                    The Cloudenly infrastructure is built on the Quantum OS with
                    a unified data kernel serving all of her applications. This
                    empowers us to meet you where you are and allows you scale
                    as your business grows without losing a single data.
                  </div>
                </div>
                <div class="flex-1 card-img-right scalability-bg">
                  <img src="/img/scalability-img.svg" />
                </div>
              </div>
            </v-tab-item>
            <v-tab-item>
              <div class="md:flex round-card" style="margin-top: 56px">
                <div class="flex-2 card-text-div">
                  <div class="card-header">Ecosystem</div>
                  <div class="card-inner-text">
                    Regardless of which application you use, the Cloudenly
                    platform keeps you connected to the global network of
                    buyers, suppliers, facilitators, and advisors, extending
                    your reach and opportunities exponentially.
                  </div>
                </div>
                <div class="flex-1 card-img-right ecosystem-bg">
                  <img src="/img/ecosystem-img.svg" />
                </div>
              </div>
            </v-tab-item>
          </v-tabs-items>
        </div>
      </div>
    </div>
  </div>
</template>
<script>
import { VTabs, VTab, VTabItem, VTabsItems } from 'vuetify/lib'
export default {
  components: {
    VTabItem,
    VTabsItems,
    VTabs,
    VTab,
  },
  data() {
    return {
      innovationText:
        'Our magic lies in our vision, craft, and the courage to shape tomorrow, in catalyzing innovation for growth. From the very first code, our mission remains the same, to provide your business with the tools that it needs to thrive.',
      tab: null,
      items: ['Innovation', 'Scalability', 'Ecosystem'],
      text:
        'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.',
    }
  },
}
</script>
<style scoped>
.why-cloudenly {
  background: #ffffff;
  box-shadow: 0px 2px 10px rgba(47, 48, 97, 0.1);
  border-radius: 10px;
  padding-top: 30px;
  text-align: center;
  padding-bottom: 56px;
}
.product-wrapper {
  background: rgb(241, 245, 251, 0.4);
  padding-left: 60px;
  padding-right: 60px;
  padding-bottom: 100px;
}
.section-name {
  font-family: GalanoGrotesque;
  font-size: 48px;
  line-height: 80px;
  color: #031a40;
}
.section-content {
  max-width: 501px;
  text-align: left;
  margin-top: 25px;
}
.section-text {
  font-family: GalanoGrotesque;
  font-size: 20px;
  line-height: 23px;
  color: #343434;
}
.innovation-text {
  font-family: GalanoGrotesque;
  font-size: 48px;
  line-height: 80px;
  color: #4781dc;
}

.basil {
  background-color: #fffbe6 !important;
}
.basil--text {
  color: #356859 !important;
}
.tabs-wrapper {
  margin-top: 27px;
  flex-direction: column;
  align-items: center;
}
.section-tabs {
  /* width: 700px; */
}
.round-card {
  background: #efefef;
  border: 4px solid #ffffff;
  box-sizing: border-box;
  border-radius: 37px;
  max-width: 1179px;
}
.card-text-div {
  height: 570px;
  padding: 149px 53px 0px 59px;
}
.card-header {
  font-family: GalanoGrotesque;
  font-size: 48px;
  line-height: 80px;
  color: #333333;
  text-align: left;
}
.card-inner-text {
  font-family: GalanoGrotesque;
  margin-top: 33px;
  font-size: 18px;
  line-height: 21px;
  color: #8e8e8e;
  max-width: 615px;
  text-align: left;
}
.card-img-right {
  width: 438px;
  height: 570px;
  /* border: 4px solid #ffffff; */
  box-sizing: border-box;
  border-radius: 0px 35px 35px 0px;
  padding-top: 97px;
  display: flex;
  justify-content: center;
}
.scalability-bg {
  background: linear-gradient(180deg, #47c9fa 0%, #4881db 100%);
}
.ecosystem-bg {
  background: linear-gradient(180deg, #ffa35d 0%, #fe6c76 100%);
}
</style>
<style>
.section-tabs .v-tabs-slider-wrapper .v-tabs-slider {
  background-color: #4781dc;
}
.section-tabs .v-tab.v-tab--active {
  color: #4781dc;
}
.section-tabs .v-tab {
  font-size: 20px;
  line-height: 23px;
}
</style>
