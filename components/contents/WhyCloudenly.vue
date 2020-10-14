/* eslint-disable prettier/prettier */
<template>
  <div>
    <div class="product-wrapper">
      <div class="why-cloudenly">
        <div class="cloudenly-headline">Why Cloudenly?</div>
        <div class="w-full sm:flex justify-center tabs-wrapper">
          <div class="section-tabs">
            <v-tabs
              v-model="tab"
              background-color="transparent"
              color="basil"
              grow
            >
              <v-tab v-for="item in items" :key="item">
                <span style="font-size: 16px; text-transform: capitalize">
                  {{ item }}</span
                >
              </v-tab>
            </v-tabs>
          </div>
          <v-tabs-items v-model="tab">
            <v-tab-item>
              <div class="md:flex round-card" style="margin-top: 56px">
                <div class="flex-2 card-text-div">
                  <div class="card-header">Innovation</div>
                  <div class="card-inner-text">
                    Our magic lies in our vision, craft, and the courage to
                    shape tomorrow,in catalyzing innovation for growth. From the
                    very first code, our mission remains the same, to provide
                    your business with the tools that it needs to thrive.
                  </div>
                </div>
                <div class="flex-1 card-img-right scalability-bg">
                  <img
                    src="/img/innovation_icon.svg"
                    class="why-cloudenly-img"
                  />
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
                  <img
                    src="/img/scalability-icon.svg"
                    class="why-cloudenly-img"
                  />
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
                  <img
                    src="/img/ecosystem-icon.svg"
                    class="why-cloudenly-img"
                  />
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
// import { VTabs, VTab, VTabItem, VTabsItems } from 'vuetify/lib'
export default {
  components: {
    // VTabItem,
    // VTabsItems,
    // VTabs,
    // VTab,
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
  /* background: #ffffff;
  box-shadow: 0px 2px 10px rgba(47, 48, 97, 0.1);
  border-radius: 10px; */

  padding-top: 30px;
  text-align: center;
  padding-bottom: 56px;
}
.product-wrapper {
  background: #ffffff;
  padding-left: 60px;
  padding-right: 60px;
  padding-bottom: 100px;
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
  font-family: GalanoGrotesque-Heavy;
  font-size: 40px;
  line-height: 80px;
  color: #333333;
  text-align: left;
}
.card-inner-text {
  margin-top: 33px;
  color: #8e8e8e;
  max-width: 615px;
  text-align: left;

  font-family: GalanoGrotesque-Medium;
  font-size: 18px;
  line-height: 21px;
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
@media (max-width: 768px) {
  .product-wrapper {
    padding-left: 1.5rem;
    padding-right: 1.5rem;
  }
  .section-content {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    padding-left: 20px;
    padding-right: 20px;
  }
  .section-text {
    text-align: center;
  }
  .innovation-text {
    font-size: 30px;
  }
  .innovation-container {
    margin-top: 30px;
    padding-bottom: 30px;
  }
  .card-text-div {
    padding: 24px 16px 40px;
    height: unset;
  }
  .card-header {
    font-size: 30px;
    text-align: center;
  }
  .card-inner-text {
    margin-top: 20px;
    text-align: center;
  }
  .card-img-right {
    width: unset;
    height: unset;
    box-sizing: border-box;
    border-radius: 0px;
    padding-top: 97px;
    display: flex;
    justify-content: center;
  }
  .why-cloudenly {
    padding-bottom: 0px;
  }
}
@media (max-width: 480px) {
  .why-cloudenly-img {
    max-width: none;
  }
}
@media (max-width: 786px) {
  .why-cloudenly-img {
    max-width: none;
  }
}
@media (max-width: 1024px) {
  .why-cloudenly-img {
    max-width: 100%;
  }
}
/* @media (max-width: 1200px) {
  .why-cloudenly-img {
    max-width: none;
  }
} */
</style>
<style>
.section-tabs .v-tabs-slider-wrapper .v-tabs-slider {
  background-color: #c4c4c4;
}
.section-tabs .v-tab.v-tab--active {
  color: #333333;
  border: 2px solid #c4c4c4;
  box-sizing: border-box;
  border-radius: 3px;
}
.section-tabs .v-tab {
  font-family: GalanoGrotesque-Medium;
  font-size: 18px;
  line-height: 80px;
  color: #333333;
}

.cloudenly-headline {
  font-size: 35px;
}
/* 
/*  *
/* @media (max-width: 768px) {
  .section-tabs .v-slide-group__wrapper {
    height: 120px;
  }
  .section-tabs .v-slide-group__content {
    flex-direction: column;
  }
  .section-tabs .v-window-item {
    margin-top: 40px;
  }
  .section-tabs .v-tabs-slider-wrapper {
    display: none;
  }
  .section-tabs .v-tab.v-tab--active {
    border: 1.5px solid #c4c4c4;
    box-sizing: border-box;
    border-radius: 4px;
    font-size: 18px;
    line-height: 80px;
    color: #333333;
  }
  .section-tabs .v-slide-group__content {
    padding: 20px;
  }
  .section-tabs .v-tab {
    padding: 12px 17px;
  }
  .section-tabs {
    margin-bottom: 50px !important;
  }
} */
</style>
