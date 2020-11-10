<template>
  <div>
    <AppHeader />
    <div>
      <section class="banner mb-8">
        <div class="content-center mr-3 ml-3">
          <h1 class="banner-h1 font-bold">How can we help you?</h1>
          <div style="max-width: 550px; margin: auto">
            <p class="banner-p font-normal">
              Find help and learning resources below
            </p>
          </div>
        </div>
      </section>
    </div>

    <main class="container mx-auto px-10 py-10">
      <div class="flex flex-wrap mt-12">
        <!-- Row One Starts here! -->
        <div class="px-4 w-full sm:w-1/2 md:w-1/3 lg:w-1/4 xl:w-1/4 mb-6">
          <nuxt-link to="/resources/product-overview">
            <div class="resource-card">
              <div class="text-center mr-3 ml-3">
                <h1 class="font-bold resources-h1 product-overview-h1">
                  Product Overview
                </h1>
                <div class="flex justify-center mt-8">
                  <img
                    class="fill-current h-16 w-16 transition duration-500 ease-in-out transform hover:-translate-y-3 hover:scale-300 ..."
                    src="~assets/resourcesIcons/product-overview.svg"
                    alt="cloudenly product overview"
                  />
                </div>

                <div style="max-width: 400px; margin: auto">
                  <p class="font-normal resources-font">
                    Read reference product overview documentation for all
                    Cloudenly's product suite
                  </p>
                </div>
              </div>
            </div>
          </nuxt-link>
        </div>

        <div class="px-4 w-full sm:w-1/2 md:w-1/3 lg:w-1/4 xl:w-1/4 mb-6">
          <nuxt-link to="/faq">
            <div class="resource-card">
              <div class="text-center mr-3 ml-3">
                <h1 class="font-bold resources-h1">FAQ</h1>
                <div style="max-width: 400px; margin: auto">
                  <div class="flex justify-center mt-8">
                    <img
                      class="fill-current h-16 w-16 transition duration-500 ease-in-out transform hover:-translate-y-3 hover:scale-300 ..."
                      src="~assets/resourcesIcons/faq.svg"
                      alt="cloudenly FAQ"
                    />
                  </div>

                  <p class="font-normal resources-font">
                    Read and find answers to frequently asked questions
                  </p>
                </div>
              </div>
            </div>
          </nuxt-link>
        </div>

        <div class="px-4 w-full sm:w-1/2 md:w-1/3 lg:w-1/4 xl:w-1/4 mb-4">
          <nuxt-link to="/resources/userguide">
            <div class="resource-card">
              <div class="text-center mr-3 ml-3">
                <h1 class="font-bold resources-h1">User Guide</h1>
                <div style="max-width: 400px; margin: auto">
                  <div class="flex justify-center mt-8">
                    <img
                      class="fill-current h-16 w-16 transition duration-500 ease-in-out transform hover:-translate-y-3 hover:scale-300 ..."
                      src="~assets/resourcesIcons/user-guide.svg"
                      alt="cloudenly userguide logo"
                    />
                  </div>
                  <p class="font-normal resources-font">
                    Read how-to articles and guides for all Cloudenly's product
                    suite
                  </p>
                </div>
              </div>
            </div>
          </nuxt-link>
        </div>
        <!-- Row Two Ends Here -->

        <div class="px-4 w-full sm:w-1/2 md:w-1/3 lg:w-1/4 xl:w-1/4 mb-6">
          <div class="resource-card">
            <div class="text-center mr-3 ml-3">
              <h1 class="font-bold resources-h1">Blog</h1>
              <div style="max-width: 400px; margin: auto">
                <div class="flex justify-center mt-8">
                  <img
                    class="fill-current h-16 w-16 transition duration-500 ease-in-out transform hover:-translate-y-3 hover:scale-300 ..."
                    src="~assets/resourcesIcons/blog.svg"
                    alt="cloudenly blog"
                  />
                </div>
                <p class="font-normal resources-font">
                  Be up to date on Cloudenly's activities as well as industry
                  and business trends
                </p>
              </div>
            </div>
          </div>
        </div>

        <div class="px-4 w-full sm:w-1/2 md:w-1/3 lg:w-1/4 xl:w-1/4 mb-6">
          <div class="resource-card events-card">
            <div class="text-center mr-3 ml-3">
              <h1 class="font-bold resources-h1">Events</h1>
              <div style="max-width: 400px; margin: auto">
                <div class="flex justify-center mt-8">
                  <img
                    class="fill-current h-16 w-16 transition duration-500 ease-in-out transform hover:-translate-y-3 hover:scale-300 ..."
                    src="~assets/resourcesIcons/events.svg"
                    alt="cloudenly events"
                  />
                </div>
                <p class="font-normal resources-font">
                  Stay up to date with events across our ecosystem
                </p>
              </div>
            </div>
          </div>
        </div>

        <div class="px-4 w-full sm:w-1/2 md:w-1/3 lg:w-1/4 xl:w-1/4 mb-6">
          <div class="resource-card">
            <div class="text-center mr-3 ml-3">
              <h1 class="font-bold resources-h1">Community</h1>
              <div style="max-width: 400px; margin: auto">
                <div class="flex justify-center mt-8">
                  <img
                    class="fill-current h-16 w-16 transition duration-500 ease-in-out transform hover:-translate-y-3 hover:scale-300 ..."
                    src="~assets/resourcesIcons/community.svg"
                    alt="cloudenly community"
                  />
                </div>
                <p class="font-normal resources-font">
                  Start a discussion, browse solutions, and get tips from us
                </p>
              </div>
            </div>
          </div>
        </div>

        <div class="px-4 w-full sm:w-1/2 md:w-1/3 lg:w-1/4 xl:w-1/4 mb-6">
          <div class="resource-card">
            <div class="text-center mr-3 ml-3">
              <h1
                style="margin-top: -68px; margin-bottom: -6px"
                class="font-bold resources-h1"
              >
                Developer Documentation
              </h1>
              <div style="max-width: 400px; margin: auto">
                <div class="flex justify-center mt-8">
                  <img
                    class="fill-current h-16 w-16 transition duration-500 ease-in-out transform hover:-translate-y-3 hover:scale-300 ..."
                    src="~assets/resourcesIcons/developer-documentation.svg"
                    alt="cloudenly developer documentation"
                  />
                </div>
                <p class="font-normal resources-font">
                  Read reference documentation for API development
                </p>
              </div>
            </div>
          </div>
        </div>

        <div class="px-4 w-full sm:w-1/2 md:w-1/3 lg:w-1/4 xl:w-1/4 mb-6">
          <div class="resource-card">
            <div class="text-center mr-3 ml-3">
              <h1 class="font-bold resources-h1">Academy</h1>
              <div style="max-width: 400px; margin: auto">
                <div class="flex justify-center mt-8">
                  <img
                    class="fill-current h-16 w-16 transition duration-500 ease-in-out transform hover:-translate-y-3 hover:scale-300 ..."
                    src="~assets/resourcesIcons/academy.svg"
                    alt="cloudenly academy"
                  />
                </div>
                <p class="font-normal resources-font">
                  Watch video trainings, take test and get certified in
                  Cloudenly's product suite
                </p>
              </div>
            </div>
          </div>
        </div>
      </div>
    </main>
    <!-- <TryCloudenlyForFree /> -->
  </div>
</template>

<script>
import AppHeader from '../../components/header/AppHeader'
// import TryCloudenlyForFree from '../../components/contents/TryCloudenlyForFree'
export default {
  components: {
    AppHeader,
    // TryCloudenlyForFree,
  },
  head() {
    return {
      title: 'Cloudenly - Resources',
      meta: [
        {
          hid: 'Cloudenly - Resources',
          name: 'Cloudenly - Resources',
          content: 'Cloudenly - Resources All you need to know.',
        },
      ],
    }
  },
}
</script>
<style scoped>
.product-overview-h1 {
  margin-top: -61px;
}
.resources-font {
  font-size: 14px;
}

* {
  font-family: GalanoGrotesque-Medium;
  color: #828282;
}
.resources-h1 {
  color: #2b2b2b;
}
.resource-card {
  border: 1px solid #cfcfcf;
  border-radius: 6px;
  padding: 80px 1px 15px 1px;
  border-radius: 6px;
  max-height: 315px;
  min-height: 285px;
}

h1 {
  line-height: 26px;
  font-size: 22px;
  font-weight: 500;
  margin-top: -50px;
}

p {
  margin-top: 38px;
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
  background-image: url('rectangle3.jpg');
  background-repeat: no-repeat;
  background-size: 100% 100%;
  color: white;
}

/* .events-card:hover {
  background: #000;
}

.events-card:hover:before {
  content: 'ADD';
} */

@media (max-width: 728px) {
  .banner-p {
    font-size: 16px;
  }

  .banner-h1 {
    font-size: 28px;
  }

  .banner {
    background-image: linear-gradient(
      269.56deg,
      #47c9fa 15.32%,
      #4881da 79.59%
    );
  }
}

@media (max-width: 480px) {
}
@media (max-width: 768px) {
}

@media (max-width: 1024px) {
}
@media (min-width: 1200px) {
}
</style>
