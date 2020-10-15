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
        <div class="px-4 w-full sm:w-1/2 md:w-1/3 lg:w-1/4 xl:w-1/4 mb-4">
          <nuxt-link to="/resources/userguide">
            <div class="resource-card bg-gray-200">
              <div class="text-center mr-3 ml-3">
                <h1 class="font-bold">User Guide</h1>
                <div style="max-width: 400px; margin: auto">
                  <p class="font-normal">
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
          <nuxt-link to="/resources/product-overview">
            <div class="resource-card bg-gray-200">
              <div class="text-center mr-3 ml-3">
                <h1 class="font-bold">Product Overview</h1>
                <div style="max-width: 400px; margin: auto; margin-top: -10px">
                  <p class="font-normal">
                    Read reference product overview documentation for all
                    Cloudenly's product suite.
                  </p>
                </div>
              </div>
            </div>
          </nuxt-link>
        </div>

        <div class="px-4 w-full sm:w-1/2 md:w-1/3 lg:w-1/4 xl:w-1/4 mb-6">
          <nuxt-link to="/">
            <div class="resource-card bg-gray-200">
              <div class="text-center mr-3 ml-3">
                <h1 class="font-bold">Blog</h1>
                <div style="max-width: 400px; margin: auto">
                  <p class="font-normal">
                    Be up to date on Cloudenly's activities as well as industry
                    and Business trends
                  </p>
                </div>
              </div>
            </div>
          </nuxt-link>
        </div>

        <div class="px-4 w-full sm:w-1/2 md:w-1/3 lg:w-1/4 xl:w-1/4 mb-6">
          <nuxt-link to="/">
            <div class="resource-card bg-gray-200">
              <div class="text-center mr-3 ml-3">
                <h1 class="font-bold">Community</h1>
                <div style="max-width: 400px; margin: auto">
                  <p class="font-normal">
                    Start a discussion, browse solutions, and get tips from us
                  </p>
                </div>
              </div>
            </div>
          </nuxt-link>
        </div>

        <div class="px-4 w-full sm:w-1/2 md:w-1/3 lg:w-1/4 xl:w-1/4 mb-6">
          <nuxt-link to="/">
            <div class="resource-card bg-gray-200">
              <div class="text-center mr-3 ml-3">
                <h1 class="font-bold">FAQ</h1>
                <div style="max-width: 400px; margin: auto">
                  <p class="font-normal">
                    Read and find answers to frequently asked questions
                  </p>
                </div>
              </div>
            </div>
          </nuxt-link>
        </div>

        <div class="px-4 w-full sm:w-1/2 md:w-1/3 lg:w-1/4 xl:w-1/4 mb-6">
          <nuxt-link to="/">
            <div class="resource-card bg-gray-200">
              <div class="text-center mr-3 ml-3">
                <h1 style="margin-bottom: -24px" class="font-bold">
                  Developer Documentation
                </h1>
                <div style="max-width: 400px; margin: auto">
                  <p class="font-normal">
                    Read reference documentation for API development
                  </p>
                </div>
              </div>
            </div>
          </nuxt-link>
        </div>

        <div class="px-4 w-full sm:w-1/2 md:w-1/3 lg:w-1/4 xl:w-1/4 mb-6">
          <nuxt-link to="/">
            <div class="resource-card bg-gray-200">
              <div class="text-center mr-3 ml-3">
                <h1 class="font-bold">Events</h1>
                <div style="max-width: 400px; margin: auto">
                  <p class="font-normal">
                    Start a discussion, browse solutions, and get tips from us
                  </p>
                </div>
              </div>
            </div>
          </nuxt-link>
        </div>

        <div class="px-4 w-full sm:w-1/2 md:w-1/3 lg:w-1/4 xl:w-1/4 mb-6">
          <nuxt-link to="/">
            <div class="resource-card bg-gray-200">
              <div class="text-center mr-3 ml-3">
                <h1 class="font-bold">Academy</h1>
                <div style="max-width: 400px; margin: auto">
                  <p class="font-normal">
                    Watch video training, take test and get certified in
                    Cloudenly's product suite
                  </p>
                </div>
              </div>
            </div>
          </nuxt-link>
        </div>
      </div>
    </main>
  </div>
</template>

<script>
import AppHeader from '../../components/header/AppHeader'
export default {
  components: {
    AppHeader,
  },
}
</script>
<style scoped>
* {
  font-family: GalanoGrotesque-Medium;
  color: #828282;
}
.resource-card {
  padding: 80px 6px 15px 6px;
  border-radius: 6px;
  min-height: 270px;
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
  padding: 15rem 0 10rem 0;
  text-align: center;
  background-image: url('rectangle3.jpg');
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
