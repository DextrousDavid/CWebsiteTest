<template>
  <div>
    <div class="sm:flex mb-4 landing-page-banner">
      <div class="sm:w-1/2 landing-page-left-div sm:flex justify-center">
        <div class="div-wrapper">
          <div class="header-text-bold">
            MAKING <b> THE SHIFT </b> IN
            <b> ENTERPRISE SOFTWARE </b>
          </div>
          <div class="header-text-light">
            Transform with Cloudenly and experience the power of a unified
            business operation.
          </div>
          <div class="call-to-action-div sm:flex">
            <button class="blue-btn">TRY FOR FREE</button>
            <button class="white-btn-border">EXPLORE MORE</button>
          </div>
        </div>
      </div>
      <div class="sm:w-1/2 landing-page-right-div flex justify-center">
        <img src="/img/frame.svg" />
      </div>
      <div class="dot-bg-top">
        <img src="/img/top-bg.svg" />
      </div>
      <div class="dot-bg-right">
        <img src="/img/right-bg.svg" />
      </div>
      <div class="dot-bottom-bg">
        <img src="/img/bottom-bg.png" />
      </div>
    </div>
    <div class="enterprices flex flex-wrap">
      <div class="trust-enterprices">
        Trusted by your favourite enterprises.
      </div>
      <div class="enterprice-box">
        <img src="/img/Mansaard-logo.svg" />
        Mansaard Inc.
      </div>
      <div class="enterprice-box">
        <img src="/img/YorkShire-logo.svg" />
        YorkShire Ent.
      </div>
      <div class="enterprice-box">
        <img src="/img/Shally-logo.svg" />
        YorkShire Ent.
      </div>
      <div class="enterprice-box">
        <img src="/img/Circle-logo.svg" />
        Circle Comp
      </div>
    </div>
    <div class="cloudenly-suite sm:flex">
      <div class="div-cover">
        <div class="cloudenly-text-suite">Cloudenly Suite</div>
        <div class="text-below">
          Our Product help your team work from anywhere delivering exceptional
          customer experiences.
        </div>
        <!-- <div class="arrow-direction flex">
          <div class="arrow-left" style="margin-right: 60px" @click="previous">
            <img src="/img/left-arrow.svg" />
          </div>
          <div class="arrow-left" @click="next">
            <img src="/img/right-arrow.svg" />
          </div>
        </div> -->
      </div>
      <!-- Slider Started -->
      <div class="products-container sm:flex">
        <hooper :items-to-show="3">
          <slide>
            <div class="product-div">
              <div class="product-top-line optima-top"></div>
              <div class="product-desc">
                <img src="/img/Optima-logo.svg" />
                <div class="product-name">Optima</div>
                <div class="product-explain">
                  An Integrated Cloud ERP for Accounting, Supply Chain and
                  Unified Commerce Solution.
                </div>
                <div class="product-learn-more">Learn More</div>
                <button class="product-btn optima-btn">TRY FOR FREE</button>
              </div>
            </div>
          </slide>
          <slide>
            <div class="product-div">
              <div class="product-top-line humana-top"></div>
              <div class="product-desc">
                <img src="/img/Humana-logo.svg" />
                <div class="product-name">HumanaR</div>
                <div class="product-explain">
                  A digital HR system for seamless HR Operations and Payroll
                  compliance.
                </div>
                <div class="product-learn-more">Learn More</div>
                <button class="product-btn humana-btn">TRY FOR FREE</button>
              </div>
            </div>
          </slide>
          <slide>
            <div class="product-div">
              <div class="product-top-line dome-top"></div>
              <div class="product-desc">
                <img src="/img/Dome-logo.svg" />
                <div class="product-name">Dome</div>
                <div class="product-explain">
                  A cloud file storage and collaboration tool. Keep track of
                  changes and restrict access.
                </div>
                <div class="product-learn-more">Learn More</div>
                <button class="product-btn dome-btn">TRY FOR FREE</button>
              </div>
            </div>
          </slide>
          <hooper-navigation slot="hooper-addons"></hooper-navigation>
          <hooper-pagination slot="hooper-addons"></hooper-pagination>
        </hooper>
      </div>
      <!-- Slider Stopped -->
    </div>
    <WhyCloudenly />
    <div class="high-growth-companies sm:flex justify-center">
      <div class="cloudenly-headline">
        Powering Growth for Amazing Businesses.
      </div>
      <div
        class="sm:flex justify-center brand-wrapper"
        style="margin-top: 30px"
      >
        <div class="company-div"><img src="/img/aws.png" /></div>
        <div class="company-div"><img src="/img/beans.png" /></div>
        <div class="company-div"><img src="/img/oya.png" /></div>
        <div class="company-div"><img src="/img/microsoft.png" /></div>
        <div class="company-div"><img src="/img/slack.png" /></div>
      </div>
      <button class="blue-btn all-brand-btn">SEE ALL BRANDS</button>
    </div>
    <ProductPackComponent />
    <div class="try-product-free sm:flex justify-center">
      <div class="cloudenly-headline">Try Cloudenly for free.</div>
      <div class="free-try-text">
        No software installation required, no credit card required, easy to
        setup.
      </div>
      <button class="blue-btn free-try-btn">TRY FOR FREE</button>
    </div>
  </div>
</template>

<script>
import { Hooper, Slide, Navigation as HooperNavigation } from 'hooper'
import WhyCloudenly from '../components/contents/WhyCloudenly'
import ProductPackComponent from '../components/contents/ProductPackComponent'
import 'hooper/dist/hooper.css'
export default {
  components: {
    WhyCloudenly,
    ProductPackComponent,
    Hooper,
    Slide,
    HooperNavigation,
  },
  data() {
    return {
      frame: 3,
      rightArrow: true,
      leftArrow: false,
      scrollWidth: 0,
      count: 0,
    }
  },
  methods: {
    previous() {
      // this.portArrowRight=true;
      this.count--
      this.count = this.count--
      this.scroll('previous')
    },
    next() {
      // this.portArrowLeft=true;
      this.count++
      this.count = this.count++
      this.scroll('next')
    },
    scroll(position) {
      const el = document.getElementById('slide')
      let pos = 0
      const id = setInterval(frame, 5)
      const num = 3 - this.frame
      const width = 200
      const resize = num * width
      const check = position === 'reset' ? resize : width
      // var obj=this;
      function frame() {
        if (pos === check) {
          clearInterval(id)
        } else {
          pos += 5
          if (position === 'next') {
            el.scrollLeft += 5
          } else {
            el.scrollLeft -= 5
          }
          // obj.portfolioScroll(el.scrollLeft);
        }
      }
    },
  },
}
</script>

<style scoped>
@media (max-width: 768px) {
  .white-btn-border {
    margin-top: 20px;
  }
  .header-text-light {
    margin-top: 20px;
  }
}
</style>
