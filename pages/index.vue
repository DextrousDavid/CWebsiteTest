<template>
  <div>
    <AppHeader />
    <div class="sm:flex mb-4 landing-page-banner">
      <div class="sm:w-1/2 landing-page-left-div sm:flex justify-center">
        <div class="div-wrapper">
          <div class="bold-header">
            The Business
            <span>Software</span>
            for a Connected Digital Economy
          </div>
          <div class="light-text-header top-text">
            Transform with Cloudenly and experience the power of a unified
            business operation.
          </div>
          <div class="light-text-header bottom-text">
            CRM. Sales. Purchase. Inventory. Operations. Commerce. Finance.
            Cloud Storage. HRM.
          </div>
          <div class="call-to-action-div sm:flex"></div>
          <button
            class="bg-blue-500 hover:bg-blue-700 text-white mr-2 py-2 px-6 rounded inline-block"
          >
            TRY FOR FREE
          </button>
          <button class="white-btn-border inline-block">EXPLORE MORE</button>
        </div>
      </div>
      <div class="sm:w-1/2 landing-page-right-div flex">
        <img src="/img/mana-img.svg" />
      </div>
    </div>

    <div class="enterprices flex flex-wrap sm:text-center">
      <div class="flex trust-enterprices md:text-left">
        Trusted by your favourite enterprises.
      </div>
      <div class="enterprice-box md:text-center">
        <img src="/img/Mansaard-logo.svg" />
        Mansaard Inc.
      </div>
      <div class="enterprice-box sm:flex">
        <img src="/img/YorkShire-logo.svg" />
        YorkShire Ent.
      </div>
      <div class="enterprice-box sm:flex">
        <img src="/img/Shally-logo.svg " />
        YorkShire Ent.
      </div>
      <div class="enterprice-box sm:flex">
        <img src="/img/Circle-logo.svg " />
        Circle Comp
      </div>
      <div class="sm:flex">
        <img src="/img/chat-icon.svg " />
      </div>
    </div>

    <div class="cloudenly-suite">
      <div class="cloudenly-headline">Cloudenly Suite</div>
      <div class="cloudenly-light-headline container">
        Our Product help your team work from anywhere delivering exceptional
        customer experiences.
      </div>
      <div class="container">
        <div class="row">
          <div class="col-sm-12 col-md-4 col-lg-4">
            <div class="product-div-lite">
              <div class="product-top-line optima-top"></div>
              <div class="product-desc">
                <img src="/img/Optima-logo.svg" />
                <div class="product-name">Optima</div>
                <div class="product-explain">
                  Streamline your retail, supply chain, commerce, finance, and
                  accounting for improved customer experience, operational
                  efficiency, business intelligence, and agility.
                </div>
                <button class="product-btn optima-btn">TRY FOR FREE</button>
              </div>
            </div>
          </div>

          <div class="col-sm-12 col-md-4 col-lg-4">
            <div class="product-div-lite">
              <div class="product-top-line humana-top"></div>
              <div class="product-desc">
                <img src="/img/Humana-logo.svg" />
                <div class="product-name">HumanaR</div>
                <div class="product-explain">
                  Amplify your HR processes with ease, and achieve better
                  employee experience with self-service. Improve people and
                  business performance through workforce analytics.
                </div>
                <button class="product-btn humana-btn">TRY FOR FREE</button>
              </div>
            </div>
          </div>

          <div class="col-sm-12 col-md-4 col-lg-4">
            <div class="product-div-lite">
              <div class="product-top-line dome-top"></div>
              <div class="product-desc">
                <img src="/img/Dome-logo.svg" />
                <div class="product-name">Dome</div>
                <div class="product-explain" style="max-width: 247px">
                  Manage files and folders securely on the cloud and collaborate
                  remotely. Enjoy the boundless opportunity.
                </div>
                <button class="product-btn dome-btn">TRY FOR FREE</button>
              </div>
            </div>
          </div>
        </div>
        <div class="row">
          <div class="col align-self-center">
            <div class="product-div-lite lite-margin">
              <div class="product-top-line lite-top"></div>
              <div class="product-desc">
                <img src="/img/Optima-logo.svg" />
                <div class="product-name">Lite</div>
                <div class="product-explain">
                  Built for micro and small businesses, to unify purchase,
                  inventory, sales, customer, expense management, and more.
                  Scaling from Lite to other Apps is seamless.
                </div>
                <button class="product-btn lite-btn">TRY FOR FREE</button>
              </div>
            </div>
          </div>
        </div>
      </div>
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
      <div class="flex justify-center font-medium">
        <button class="all-brand-btn mt-4">SEE ALL BRANDS</button>
      </div>
    </div>
    <ProductPackComponent />
    <div class="try-product-free sm:flex justify-center">
      <div class="cloudenly-headline">Try Cloudenly for free.</div>
      <div class="free-try-text">
        No software installation required, no credit card required, easy to
        setup.
      </div>
      <div class="flex justify-center">
        <button class="all-brand-btn mt-4 font-medium">TRY FOR FREE</button>
      </div>
    </div>
  </div>
</template>

<script>
import AppHeader from '../components/header/AppHeader'
import WhyCloudenly from '../components/contents/WhyCloudenly'
import ProductPackComponent from '../components/contents/ProductPackComponent'
export default {
  components: {
    AppHeader,
    WhyCloudenly,
    ProductPackComponent,
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
.container {
  width: 100%;
  padding: 12px;
  margin-right: 70px;
  margin-left: auto;
}
@media (max-width: 480px) {
  .why-cloudenly-img {
    max-width: none;
  }
  .product-div-lite {
    background: #ffffff;
    box-shadow: 0px 2px 10px rgba(47, 48, 97, 0.1);
    border-radius: 8px;
    max-width: 278px;
    margin: auto;
    padding-bottom: 34px;
  }
}
@media (max-width: 768px) {
  .white-btn-border {
    margin-top: 20px;
  }
  .header-text-light {
    margin-top: 20px;
  }
  .product-div-lite {
    background: #ffffff;
    box-shadow: 0px 2px 10px rgba(47, 48, 97, 0.1);
    border-radius: 8px;
    max-width: 278px;
    margin: auto;
    padding-bottom: 34px;
  }
}

@media (max-width: 1024px) {
  .why-cloudenly-img {
    max-width: 100%;
  }
  .product-div-lite {
    background: #ffffff;
    box-shadow: 0px 2px 10px rgba(47, 48, 97, 0.1);
    border-radius: 8px;
    max-width: 270px;
    margin: auto;
    padding-bottom: 34px;
  }
}
@media (min-width: 1200px) {
  .why-cloudenly-img {
    max-width: none;
  }
  .product-div-lite {
    background: #ffffff;
    box-shadow: 0px 2px 10px rgba(47, 48, 97, 0.1);
    border-radius: 8px;
    max-width: 370px;
    margin: auto;
    padding-bottom: 34px;
  }
}
</style>
