<template>
  <div>
    <AppHeader />
    <div>
      <section class="banner mb-8">
        <div class="content-center mr-3 ml-3">
          <h1 class="banner-h1 font-bold">How can we help you?</h1>
          <div style="max-width: 550px; margin: auto">
            <p class="banner-p font-normal">
              Flexible pricing options, from personal projects to enterprise
              applications, and everything in between.
            </p>
          </div>

          <span class="content-center">
            <Inputform />
          </span>
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
                    Start a discussion, browse solutions, and get tips from us
                  </p>
                </div>
              </div>
            </div>
          </nuxt-link>
        </div>
        <!-- Row Two Ends Here -->
        <div class="px-4 w-full sm:w-1/2 md:w-1/3 lg:w-1/4 xl:w-1/4 mb-6">
          <nuxt-link to="/resources/whitepaper">
            <div class="resource-card bg-gray-200">
              <div class="text-center mr-3 ml-3">
                <h1 class="font-bold">White Paper</h1>
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
                <h1 class="font-bold">Blog</h1>
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
                <h1 style="margin-bottom: -24px" class="font-bold">
                  Developer Documentation
                </h1>
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
                    Start a discussion, browse solutions, and get tips from us
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
import Inputform from '../../components/contents/Inputform'
import AppHeader from '../../components/header/AppHeader'
export default {
  components: {
    Inputform,
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
}

h1 {
  line-height: 26px;
  font-size: 22px;
  font-weight: 500;
  margin-top: -50px;
}

p {
  margin-top: 120px;
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
  padding: 13rem 0 5rem 0;
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
</style>
