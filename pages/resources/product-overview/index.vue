<template>
  <no-ssr>
    <!-- No ssr goes in here,cant use <client-only> nuxt is v2.14 -->
    <div>
      <!-- Banner goes in here -->
      <UserguideHeader />
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

      <div class="mt-16 mb-10 flex items-center justify-center">
        <div class="font-extrabold rounded-lg">
          <img
            class="-mb-4 img-logo text-center inline-block fill-current h-20 w-20"
            src="~assets/Cloudenly.svg"
            alt="cloudenly Logo"
          />
          <span class="logoTexts">
            <h1 class="font-extrabold h1-logo inline-block" style="color: #333">
              Cloudenly
            </h1>
            <h3 class="-mt-2 text-center font-semibold">Product Overview</h3>
          </span>
        </div>
      </div>

      <!-- main content -->
      <main class="container mx-auto px-10 py-10">
        <div class="flex flex-wrap">
          <!-- Row One Starts here! -->
          <div class="px-8 w-full sm:w-1/2 md:w-1/3 lg:w-1/3 xl:w-1/3 mb-4">
            <a href="https://resources.cloudenly.com/optima/">
              <div class="resource-card shadow-md">
                <div class="text-center mr-3 ml-3">
                  <!-- <h1 class="font-bold">User Guide</h1> -->
                  <div style="max-width: 300px; margin: auto">
                    <img
                      class="userguideicons transition duration-500 ease-in-out transform hover:-translate-y-3 hover:scale-300 ..."
                      src="~assets/userguideIcons/Optima1.png"
                      alt="optima logo"
                    />
                    <h5 class="font-semibold">Optima</h5>
                  </div>
                </div>
              </div>
            </a>
          </div>
          <!-- Row 1 Ends Here -->

          <div class="px-8 w-full sm:w-1/2 md:w-1/3 lg:w-1/3 xl:w-1/3 mb-4">
            <a href="https://resources.cloudenly.com/humanar/">
              <div class="resource-card shadow-md">
                <div class="text-center mr-3 ml-3">
                  <!-- <h1 class="font-bold">User Guide</h1> -->
                  <div style="max-width: 300px; margin: auto">
                    <img
                      class="userguideicons transition duration-500 ease-in-out transform hover:-translate-y-3 hover:scale-300 ..."
                      src="~assets/userguideIcons/HumanaR.png"
                      alt="humanaR logo"
                    />
                    <h5 class="font-semibold">HumanaR</h5>
                  </div>
                </div>
              </div>
            </a>
          </div>

          <div class="px-8 w-full sm:w-1/2 md:w-1/3 lg:w-1/3 xl:w-1/3 mb-4">
            <a href="https://resources.cloudenly.com/dome/">
              <div class="resource-card shadow-md">
                <div class="text-center mr-3 ml-3">
                  <!-- <h1 class="font-bold">User Guide</h1> -->
                  <div style="max-width: 300px; margin: auto">
                    <img
                      class="userguideicons transition duration-500 ease-in-out transform hover:-translate-y-3 hover:scale-300 ..."
                      src="~assets/userguideIcons/Dome.png"
                      alt="Dome logo"
                    />
                    <h5 class="font-semibold">Dome</h5>
                  </div>
                </div>
              </div>
            </a>
          </div>

          <div class="px-8 w-full sm:w-1/2 md:w-1/3 lg:w-1/3 xl:w-1/3 mb-4">
            <a href="https://resources.cloudenly.com/ally/">
              <div class="resource-card shadow-md">
                <div class="text-center mr-3 ml-3">
                  <!-- <h1 class="font-bold">User Guide</h1> -->
                  <div style="max-width: 300px; margin: auto">
                    <img
                      class="userguideicons transition duration-500 ease-in-out transform hover:-translate-y-3 hover:scale-300 ..."
                      src="~assets/userguideIcons/Ally.png"
                      alt="Ally logo"
                    />
                    <h5 class="font-semibold">Ally</h5>
                  </div>
                </div>
              </div>
            </a>
          </div>

          <div class="px-8 w-full sm:w-1/2 md:w-1/3 lg:w-1/3 xl:w-1/3 mb-4">
            <a href="https://resources.cloudenly.com/quantum/">
              <div class="resource-card shadow-md">
                <div class="text-center mr-3 ml-3">
                  <!-- <h1 class="font-bold">User Guide</h1> -->
                  <div style="max-width: 300px; margin: auto">
                    <img
                      class="userguideicons transition duration-500 ease-in-out transform hover:-translate-y-3 hover:scale-300 ..."
                      src="~assets/userguideIcons/Quantum.png"
                      alt="Quantum logo"
                    />
                    <h5 class="font-semibold">Quantum</h5>
                  </div>
                </div>
              </div>
            </a>
          </div>

          <div class="px-8 w-full sm:w-1/2 md:w-1/3 lg:w-1/3 xl:w-1/3 mb-4">
            <a href="https://resources.cloudenly.com/lite/">
              <div class="resource-card shadow-md">
                <div class="text-center mr-3 ml-3">
                  <!-- <h1 class="font-bold">User Guide</h1> -->
                  <div style="max-width: 300px; margin: auto">
                    <img
                      class="userguideicons transition duration-500 ease-in-out transform hover:-translate-y-3 hover:scale-300 ..."
                      src="~assets/userguideIcons/Lite.png"
                      alt="Lite logo"
                    />
                    <h5 class="font-semibold">Lite</h5>
                  </div>
                </div>
              </div>
            </a>
          </div>
        </div>
      </main>
      <!-- <TryCloudenlyForFree /> -->
    </div>
  </no-ssr>
</template>

<script>
import UserguideHeader from '../../../components/contents/UserguideHeader'
// import TryCloudenlyForFree from '../../../components/contents/TryCloudenlyForFree'
// import Banner from '../../../components/contents/Banner'

export default {
  components: {
    UserguideHeader,
    // Banner,
    // TryCloudenlyForFree,
  },
  head() {
    return {
      title: 'Cloudenly - Product Overview',
      meta: [
        {
          hid: 'Cloudenly - Product Overview',
          name: 'Cloudenly - Product Overview',
          content: 'Welcome to Product Overview page',
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

h3 {
  margin-left: 5rem;
}

.resource-card {
  padding: 30px 8px 15px 8px;
  border-radius: 6px;
  border: 2px solid #f4f4f4;
  margin-bottom: 40px;
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
