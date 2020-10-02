/* eslint-disable */
<template>
  <div>
    <div class="sm:flex product-wrapper">
      <hr class="vertical-divider" />
      <div class="center-div-icons">
        <img src="/img/icon-right.svg" />
        <div class="horizontal-line"></div>
        <img src="/img/icon-left.svg" style="margin-left: 47px" />
      </div>
      <div class="sm:w-1/2 product-features-left flex justify-center">
        <div class="card-feature">
          <div class="feature-header">{{ features[0].header }}</div>
          <div class="feature-description-left">
            {{ features[0].content }}
          </div>
          <div class="feature-icons-left flex justify-items-end">
            <img src="/img/icon-1.svg" />
            <img src="/img/icon-2.svg" />
            <img src="/img/icon-3.svg" />
            <img src="/img/icon-4.svg" />
          </div>
        </div>
        <div class="card-feature">
          <div class="feature-header">{{ features[1].header }}</div>
          <div class="feature-description-left">
            {{ features[0].content }}
          </div>
          <div class="feature-icons-left flex justify-items-end">
            <img src="/img/icon-1.svg" />
            <img src="/img/icon-2.svg" />
            <img src="/img/icon-3.svg" />
            <img src="/img/icon-4.svg" />
          </div>
        </div>
        <div class="card-feature">
          <div class="feature-header">{{ features[2].header }}</div>
          <div class="feature-description-left">
            {{ features[2].content }}
          </div>
          <div class="feature-icons-left flex justify-items-end">
            <img src="/img/icon-1.svg" />
            <img src="/img/icon-2.svg" />
            <img src="/img/icon-3.svg" />
            <img src="/img/icon-4.svg" />
          </div>
        </div>
        <div v-if="features[3].header" class="card-feature">
          <div class="feature-header">{{ features[3].header }}</div>
        </div>
      </div>
      <div class="sm:w-1/2 product-features-right flex justify-center">
        <div class="card-feature">
          <div class="feature-header">{{ features[4].header }}</div>
          <div class="feature-description-right">
            {{ features[4].content }}
          </div>
          <div class="feature-icons-right flex justify-items-end">
            <img src="/img/icon-1.svg" />
            <img src="/img/icon-2.svg" />
          </div>
        </div>
        <div class="card-feature">
          <div class="feature-header">{{ features[5].header }}</div>
          <div class="feature-description-right">
            {{ features[5].content }}
          </div>
          <div class="feature-icons-right flex justify-items-end">
            <img src="/img/icon-1.svg" />
            <img src="/img/icon-2.svg" />
            <img src="/img/icon-3.svg" />
            <img src="/img/icon-4.svg" />
          </div>
        </div>
        <div v-if="features[6]" class="card-feature">
          <div class="feature-header">{{ features[6].header }}</div>
          <div class="feature-description-right">
            {{ features[6].content }}
          </div>
          <div class="feature-icons-right flex justify-items-end">
            <img src="/img/icon-1.svg" />
            <img src="/img/icon-2.svg" />
            <img src="/img/icon-3.svg" />
            <img src="/img/icon-4.svg" />
          </div>
        </div>
        <div v-if="features[7]" class="card-feature">
          <div class="feature-header">{{ features[7].header }}</div>
          <div v-if="features[7].content" class="feature-description-right">
            {{ features[7].content }}
          </div>
        </div>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  props: {
    features: Array,
  },
  data() {
    return {}
  },
}
</script>
<style scoped>
/* Product Card */
.product-wrapper {
  /* background-color: rgb(241, 245, 251, 0.4); */
  background: #f9fbfd;
  border: 5px solid #ffffff;
  border-radius: 15px;
  margin-top: 30px;
  width: 1304px;
  /* height: 792px; */
  padding: 50px 80px;
  position: relative;
}
.product-features-left {
  flex-direction: column;
  /* align-items: center; */
}
.product-features-right {
  flex-direction: column;
  /* align-items: center; */
  align-items: flex-end;
}
.card-feature {
  width: 430px;
  text-align: right;
  margin-bottom: 30px;
}
.feature-header {
  font-family: GalanoGrotesque-Medium;
  font-size: 18px;
  line-height: 21px;

  color: #333333;
}
.feature-description-left {
  font-family: GalanoGrotesque-Medium;
  font-size: 16px;
  line-height: 19px;
  text-align: right;
  color: #8e8e8e;
  margin-top: 5px;
}
.feature-description-right {
  font-family: GalanoGrotesque-Medium;
  font-size: 16px;
  line-height: 19px;
  text-align: left;
  color: #8e8e8e;
  margin-top: 5px;
}
.feature-icons-right {
  margin-top: 15px;
}
.feature-icons-left {
  justify-content: flex-end;
  margin-top: 15px;
}
.feature-icons-left img {
  margin-left: 16px;
}
.feature-icons-right img {
  margin-right: 16px;
}
.vertical-divider {
  position: absolute;
  left: 50%;
  top: 5%;
  bottom: 5%;
  width: 4px;
  height: 90%;
  /* height: 100%; */
  background: #4c9f70;
}
.horizontal-line {
  /* width: 4px; */
  /* background: #4c9f70; */
  border-bottom: solid 4px #4c9f70;
  top: 48%;
  right: 51px;
  width: 61px;
  position: absolute;
}
.product-features-right .feature-header {
  text-align: left;
}
.center-div-icons {
  display: flex;
  width: 170px;
  position: absolute;
  top: 40%;
  left: 43.3%;
}

@media (max-width: 768px) {
  .product-wrapper {
    background-color: rgb(241, 245, 251, 0.4);
    border: 5px solid #ffffff;
    border-radius: 15px;
    margin-top: 30px;
    width: unset;
    height: unset;
    padding: 20px 15px;
    position: relative;
  }
  .card-feature {
    width: unset;
    display: flex;
    flex-direction: column;
    /* justify-content: center; */
    align-items: center;
  }
  .feature-description-left,
  .feature-header {
    text-align: center;
  }

  .feature-icons-left {
    justify-content: center;
  }
  .vertical-divider,
  .center-div-icons {
    display: none;
  }
  .card-feature {
    margin-bottom: 45px;
  }
  .product-features-right {
    align-items: unset;
  }
  .feature-header {
    text-align: center;
  }
  .product-features-right .feature-header,
  .feature-description-right {
    text-align: center;
  }
}
</style>
