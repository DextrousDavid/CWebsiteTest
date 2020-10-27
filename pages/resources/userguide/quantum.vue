<template>
  <div>
    <UserguideHeader />
    <Banner />
    <div class="mt-12 mb-8 flex items-center text-center justify-center">
      <div class="rounded-lg">
        <img
          class="mr-3 inline-block"
          src="~assets/userguideIcons/Quantum.png"
          alt="QuantumLogo"
        />
        <h1 class="font-bold inline-block" style="color: #333">Quantum</h1>
        <!-- The one below Doesnt look to Good -->
        <!-- <h2 class="-ml-24 my-3">User Guide</h2> -->
        <h3 class="-mt-2 font-semibold" style="color: #333">User Guide</h3>
      </div>
    </div>

    <!-- main content -->
    <main class="container sm:mx-auto">
      <!-- <Accordion /> -->
    </main>
  </div>
</template>

<script>
import Banner from '../../../components/contents/Banner'
import UserguideHeader from '../../../components/contents/UserguideHeader'
// // import Accordion from '../../components/Accordion'

export default {
  components: {
    UserguideHeader,
    Banner,
    // Accordion,
  },
  head() {
    return {
      title: 'User Guide - Quantum',
      meta: [
        {
          hid: 'User Guide - Quantum',
          name: 'User Guide - Quantum',
          content: 'Tips and Tricks of Quantum, Get started with Quantum.',
        },
      ],
    }
  },
}
</script>

<style scoped>
* {
  font-family: 'GalanoGrotesque-Regular', 'Quicksand', 'Source Sans Pro',
    -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, 'Helvetica Neue',
    Arial, sans-serif;
}

h1 {
  font-size: 40px;
  margin-bottom: -20px;
  margin-left: -8px;
}

h2 {
  font-size: 20px;
}

img {
  margin-top: -28px;
  height: 80px;
}
/* .resource-card {
  padding: 40px 6px 15px 6px;
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

h5 {
  margin-top: 20px;
  font-size: 14px;
  margin-bottom: 20px;
}

.userguideicons {
  width: 50%;
  margin: auto;
} */
</style>
