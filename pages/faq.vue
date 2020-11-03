<template>
  <no-ssr>
    <div>
      <AppHeader />
      <!-- Remove shadow outline to remove outlines that appears when you click on a button or input (Focus focus:shadow-outline?) === focus:outline-none -->
      <!-- Banner Starts here -->
      <section class="banner mb-8">
        <div class="content-center mr-3 ml-3">
          <h1 class="banner-h1">Frequently Asked Questions</h1>
          <div style="max-width: 550px; margin: auto">
            <!-- <p class="banner-p font-normal">
            Our technical teams are currently facing a significant increase in
            the number of support requests. You may experience a delayed
            response time as we work to address this.
          </p> -->
          </div>
        </div>
      </section>
      <!-- Banner Ends here -->
      <div class="mt-12 mb-8 flex items-center text-center justify-center">
        <div class="rounded-lg">
          <img
            style="width: 13rem"
            src="/img/cloudenly-logo.svg"
            alt="Cloudenlylogo"
          />

          <!-- The one below Doesnt look to Good -->
          <!-- <h2 class="-ml-24 my-3">User Guide</h2> -->
          <!-- <h3 class="ml-8 -mt-2 font-semibold">User Guide</h3> -->
        </div>
      </div>
      <main>
        <no-ssr>
          <Accordion :user-guides="userGuides" />
        </no-ssr>
      </main>
    </div>
  </no-ssr>
</template>

<script>
import AppHeader from './../components/header/AppHeader'
import Accordion from './../components/contents/Accordion'
export default {
  components: {
    AppHeader,
    Accordion,
  },
  data() {
    return {
      userGuides: [
        {
          id: 1,
          heading: 'Cloudenly',
          content1:
            'Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sit tortor, erat etiam auctor nunc, varius viverra sem. Sit nunc interdum pharetra, fringilla. In justo, pretium pellentesque est nisl. Habitasse velit, faucibus et dictum rutrum vitae',
        },
        {
          id: 2,
          heading: 'Cloudenly',
          content1:
            'Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sit tortor, erat etiam auctor nunc, varius viverra sem. Sit nunc interdum pharetra, fringilla. In justo, pretium pellentesque est nisl. Habitasse velit, faucibus et dictum rutrum vitae',
        },
        {
          id: 3,
          heading: 'Cloudenly',
          content1:
            'Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sit tortor, erat etiam auctor nunc, varius viverra sem. Sit nunc interdum pharetra, fringilla. In justo, pretium pellentesque est nisl. Habitasse velit, faucibus et dictum rutrum vitae',
        },
        {
          id: 4,
          heading: 'Cloudenly',
          content1:
            'Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sit tortor, erat etiam auctor nunc, varius viverra sem. Sit nunc interdum pharetra, fringilla. In justo, pretium pellentesque est nisl. Habitasse velit, faucibus et dictum rutrum vitae',
        },
        {
          id: 5,
          heading: 'Cloudenly',
          content1:
            'Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sit tortor, erat etiam auctor nunc, varius viverra sem. Sit nunc interdum pharetra, fringilla. In justo, pretium pellentesque est nisl. Habitasse velit, faucibus et dictum rutrum vitae',
        },
        {
          id: 7,
          heading: 'Cloudenly',
          content1:
            'Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sit tortor, erat etiam auctor nunc, varius viverra sem. Sit nunc interdum pharetra, fringilla. In justo, pretium pellentesque est nisl. Habitasse velit, faucibus et dictum rutrum vitae',
        },
        {
          id: 8,
          heading: 'Cloudenly',
          content1:
            'Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sit tortor, erat etiam auctor nunc, varius viverra sem. Sit nunc interdum pharetra, fringilla. In justo, pretium pellentesque est nisl. Habitasse velit, faucibus et dictum rutrum vitae',
        },
        {
          id: 9,
          heading: 'Cloudenly',
          content1:
            'Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sit tortor, erat etiam auctor nunc, varius viverra sem. Sit nunc interdum pharetra, fringilla. In justo, pretium pellentesque est nisl. Habitasse velit, faucibus et dictum rutrum vitae',
        },
        {
          id: 10,
          heading: 'Cloudenly',
          content1:
            'Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sit tortor, erat etiam auctor nunc, varius viverra sem. Sit nunc interdum pharetra, fringilla. In justo, pretium pellentesque est nisl. Habitasse velit, faucibus et dictum rutrum vitae',
        },
        {
          id: 11,
          heading: 'Cloudenly',
          content1:
            'Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sit tortor, erat etiam auctor nunc, varius viverra sem. Sit nunc interdum pharetra, fringilla. In justo, pretium pellentesque est nisl. Habitasse velit, faucibus et dictum rutrum vitae',
        },
      ],
    }
  },
  head() {
    return {
      title: 'Cloudenly - FAQ',
      meta: [
        {
          hid: 'Cloudenly - FAQ',
          name: ' Cloudenly - FAQ',
          content: 'Frequently Asked Questions',
        },
      ],
    }
  },
}
</script>

<style scoped>
* {
  font-family: GalanoGrotesque-Medium;
  color: #343434;
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
  font-size: 15px;
  text-align: center;
  margin: auto;
  color: #fff;
}

.banner {
  max-width: 100%;
  padding: 8rem 0 7rem 0;
  margin-top: 5rem;
  text-align: center;
  background-image: url('~assets/rectangle3.jpg');
  background-repeat: no-repeat;
  background-size: 100% 100%;
  color: white;
}

@media (max-width: 728px) {
  /* .your-subscription-code {
        width: 10%;
    } */
  .add-more-attachments-hr {
    display: none;
  }
  .banner-p {
    font-size: 14px;
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
