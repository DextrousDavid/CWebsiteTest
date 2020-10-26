<template>
  <div>
    <!-- Banner goes in here -->
    <UserguideHeader />
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

    <div class="mb-10 flex items-center justify-center">
      <!-- <nuxt-link to="/resources/userguide"> -->
      <div class="font-extrabold items-center rounded-lg">
        <img
          class="-mb-4 img-logo inline-block fill-current h-20 w-20"
          src="~assets/Cloudenly.svg"
          alt="cloudenlyLogo"
        />
        <h1 class="font-extrabold h1-logo inline-block">Cloudenly</h1>
        <h3 class="h3-logo -mt-2 text-center font-semibold">User Guide</h3>
      </div>
      <!-- </nuxt-link> -->
    </div>

    <!-- main Content -->
    <main class="container mx-auto px-10 py-10">
      <div class="flex flex-wrap">
        <!-- Row One Starts here! -->
        <div class="px-8 w-full sm:w-1/2 md:w-1/3 lg:w-1/3 xl:w-1/3 mb-4">
          <nuxt-link to="/resources/userguide/optima">
            <div class="resource-card shadow-md">
              <div class="text-center mr-3 ml-3">
                <!-- <h1 class="font-bold">User Guide</h1> -->
                <div style="max-width: 300px; margin: auto">
                  <img
                    class="userguideicons transition duration-500 ease-in-out transform hover:-translate-y-3 hover:scale-300 ..."
                    src="~assets/userguideIcons/Optima1.png"
                    alt="optima1"
                  />
                  <h5 class="font-semibold">Optima</h5>
                </div>
              </div>
            </div>
          </nuxt-link>
        </div>
        <!-- Row 1 Ends Here -->
        <div class="px-8 w-full sm:w-1/2 md:w-1/3 lg:w-1/3 xl:w-1/3 mb-4">
          <nuxt-link to="/resources/userguide/humanaR">
            <div class="resource-card shadow-md">
              <div class="text-center mr-3 ml-3">
                <!-- <h1 class="font-bold">User Guide</h1> -->
                <div style="max-width: 300px; margin: auto">
                  <img
                    class="userguideicons transition duration-500 ease-in-out transform hover:-translate-y-3 hover:scale-300 ..."
                    src="~assets/userguideIcons/HumanaR.png"
                    alt="humanaR"
                  />
                  <h5 class="font-semibold">HumanaR</h5>
                </div>
              </div>
            </div>
          </nuxt-link>
        </div>

        <div class="px-8 w-full sm:w-1/2 md:w-1/3 lg:w-1/3 xl:w-1/3 mb-4">
          <nuxt-link to="/resources/userguide/dome">
            <div class="resource-card shadow-md">
              <div class="text-center mr-3 ml-3">
                <!-- <h1 class="font-bold">User Guide</h1> -->
                <div style="max-width: 300px; margin: auto">
                  <img
                    class="userguideicons transition duration-500 ease-in-out transform hover:-translate-y-3 hover:scale-300 ..."
                    src="~assets/userguideIcons/Dome.png"
                    alt="Dome"
                  />
                  <h5 class="font-semibold">Dome</h5>
                </div>
              </div>
            </div>
          </nuxt-link>
        </div>

        <div class="px-8 w-full sm:w-1/2 md:w-1/3 lg:w-1/3 xl:w-1/3 mb-4">
          <nuxt-link to="/resources/userguide/ally">
            <div class="resource-card shadow-md">
              <div class="text-center mr-3 ml-3">
                <!-- <h1 class="font-bold">User Guide</h1> -->
                <div style="max-width: 300px; margin: auto">
                  <img
                    class="userguideicons transition duration-500 ease-in-out transform hover:-translate-y-3 hover:scale-300 ..."
                    src="~assets/userguideIcons/Ally.png"
                    alt="Ally"
                  />
                  <h5 class="font-semibold">Ally</h5>
                </div>
              </div>
            </div>
          </nuxt-link>
        </div>

        <div class="px-8 w-full sm:w-1/2 md:w-1/3 lg:w-1/3 xl:w-1/3 mb-4">
          <nuxt-link to="/resources/userguide/quantum">
            <div class="resource-card shadow-md">
              <div class="text-center mr-3 ml-3">
                <!-- <h1 class="font-bold">User Guide</h1> -->
                <div style="max-width: 300px; margin: auto">
                  <img
                    class="userguideicons transition duration-500 ease-in-out transform hover:-translate-y-3 hover:scale-300 ..."
                    src="~assets/userguideIcons/Quantum.png"
                    alt="Quantum"
                  />
                  <h5 class="font-semibold">Quantum</h5>
                </div>
              </div>
            </div>
          </nuxt-link>
        </div>

        <div class="px-8 w-full sm:w-1/2 md:w-1/3 lg:w-1/3 xl:w-1/3 mb-4">
          <nuxt-link to="/resources/userguide/lite">
            <div class="resource-card shadow-md">
              <div class="text-center mr-3 ml-3">
                <!-- <h1 class="font-bold">User Guide</h1> -->
                <div style="max-width: 300px; margin: auto">
                  <img
                    class="userguideicons transition duration-500 ease-in-out transform hover:-translate-y-3 hover:scale-300 ..."
                    src="~assets/userguideIcons/Lite.png"
                    alt="Lite"
                  />
                  <h5 class="font-semibold">Lite</h5>
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
import UserguideHeader from '../../../components/contents/UserguideHeader'
// import Banner from '../../../components/contents/Banner'

export default {
  components: {
    UserguideHeader,
    // Banner,
  },
  head() {
    return {
      title: 'Cloudenly - User Guide',
      meta: [
        {
          hid: 'Cloudenly - User Guide',
          name: 'Cloudenly - User Guide',
          content: 'Our User Guide - All you need to know',
        },
      ],
      link: [
        {
          rel: 'stylesheet',
          href:
            '//db.onlinewebfonts.com/c/0007c768c0c6149485a44a0409d9433c?family=GalanoGrotesque-Regular',
        },
      ],
    }
  },
}
</script>

<style scoped>
* {
  font-family: GalanoGrotesque-Medium;
  color: #828282;
}

.resource-card {
  padding: 30px 8px 15px 8px;
  border-radius: 6px;
  border: 2px solid #f4f4f4;
  margin-bottom: 40px;
}

h3 {
  margin-left: 2rem;
}

h1 {
  line-height: 26px;
  font-size: 22px;
  font-weight: 500;
  margin-top: -50px;
}

.h1-logo {
  font-size: 30px;
  margin-bottom: -20px;
  font-weight: 800;
  margin-left: 2px;
}

.img-logo {
  margin-top: -28px;
}
h5 {
  margin-top: 20px;
  font-size: 14px;
  margin-bottom: 20px;
}

.userguideicons {
  width: 50%;
  margin: auto;
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

@media (max-width: 728px) {
  .banner-p {
    font-size: 15px;
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
