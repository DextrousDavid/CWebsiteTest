<template>
  <no-ssr>
    <!-- <div class="user-terms-of-use-container"> -->
    <div>
      <AppHeader />
      <!-- <Banner /> -->
      <section class="banner mb-8">
        <div class="content-center mr-3 ml-3">
          <h1 class="banner-h1">Terms and Policies</h1>
          <div style="max-width: 550px; margin: auto"></div>
        </div>
      </section>

      <!-- Banner Ends here -->
      <main class="container mx-auto px-2 py-10 mt-8">
        <div class="flex flex-wrap">
          <div class="side-bar w-xs pb-4">
            <div class="flex-wrap bg-white">
              <a
                href="#"
                class="block no-underline hover:underline font-semibold text-grey-dark px-4 py-1"
                >ON THIS PAGE</a
              >
              <a
                href="#"
                class="block no-underline hover:underline text-grey-dark px-4 py-1 text-sm"
                >Customer Terms of Service</a
              >
              <a
                href="#"
                class="block no-underline hover:underline text-grey-dark px-4 py-1 text-sm"
                >User Terms of Service</a
              >
              <a
                href="#"
                class="block no-underline hover:underline text-grey-dark px-4 py-1 text-sm"
                >Customer-Specific Suppl.</a
              >
              <a
                href="#"
                class="block no-underline hover:underline text-grey-dark px-4 py-1 text-sm"
                >API Terms of Service</a
              >
              <a
                href="#"
                class="block no-underline hover:underline text-grey-dark px-4 py-1 text-sm"
                >App Directory Agreement</a
              >
              <a
                href="#"
                class="block no-underline hover:underline text-grey-dark px-4 py-1 text-sm"
                >Service Level Agreement</a
              >

              <a
                href="#"
                class="block no-underline hover:underline text-grey-dark px-4 py-1 text-sm"
                >Data Processing Agenda</a
              >
              <a
                href="#"
                class="block no-underline hover:underline text-grey-dark px-4 py-1 text-sm"
                >Slack Partner Program Terms & Condition</a
              >

              <a
                href="#"
                class="block no-underline hover:underline text-grey-dark px-4 py-1 text-sm"
                >Privacy Shield Notice</a
              >
              <a
                href="#"
                class="block no-underline hover:underline text-grey-dark px-4 py-1 text-sm"
                >Acceptable Use Policy</a
              >
              <a
                href="#"
                class="block no-underline hover:underline text-grey-dark px-4 py-1 text-sm"
                >Slack Subprocessors</a
              >
              <a
                href="#"
                class="block no-underline hover:underline text-grey-dark px-4 py-1 text-sm"
                >Slack Affiliates</a
              >
              <a
                href="#"
                class="block no-underline hover:underline text-grey-dark px-4 py-1 text-sm"
                >DMCA Policy</a
              >
              <a
                href="#"
                class="block no-underline hover:underline text-grey-dark px-4 py-1 text-sm"
                >Multi-year Accessibility Plan</a
              >
              <a
                href="#"
                class="mt-5 block no-underline hover:underline font-semibold text-grey-dark px-4 py-1"
                >SECURITY</a
              >
              <a
                href="#"
                class="block no-underline hover:underline text-grey-dark px-4 py-1 text-sm"
                >Security Practices</a
              >
              <a
                href="#"
                class="block no-underline hover:underline text-grey-dark px-4 py-1 text-sm"
                >Report a Vulnerability</a
              >

              <a
                href="#"
                class="block no-underline hover:underline text-grey-dark px-4 py-1 text-sm"
              >
                Cloudenly Certified Participant</a
              >
              <a
                href="#"
                class="block no-underline text-grey-dark px-4 py-1 text-sm"
                >Agreement</a
              >
              <!-- <a
              href="#"
              class="block no-underline hover:underline text-grey-dark px-4 py-1 text-sm"
              >Slack Partner Program Terms and Conditions</a
            > -->
            </div>
          </div>

          <!-- Resources Items starts here -->
          <div class="flex-1 flex-wrap user-terms-of-services-cards mx-5">
            <!-- Row One Starts here! -->
            <div class="md:flex mb-6">
              <div
                class="flex px-4 w-full sm:w-1/2 md:w-1/2 lg:w-1/2 xl:w-1/2 mx-auto"
                style="margin-bottom: 18px"
              >
                <div>
                  <div class="max-w-sm rounded overflow-hidden cards">
                    <div class="font-bold text-lg mb-2 px-3 pt-5">
                      Terms of Use
                    </div>
                    <div class="pb-5 px-3 text-sm">
                      This Terms of Use Agreement (this “Agreement”) is made and
                      entered into by...
                    </div>
                    <img
                      class="w-full mb-3"
                      src="~assets/policyIcons/security.png"
                      alt="security card"
                    />
                    <nuxt-link
                      to="/privacy/terms-and-policies/terms-of-use-agreement"
                      class=""
                    >
                      <div class="text-blue-500 read-more float-left pl-5 pb-4">
                        READ MORE
                      </div>
                      <div class="float-right pb-4 pr-5 mt-1 mr-2">
                        <img src="~assets/right-arrow.png" alt="right-arrow" />
                      </div>
                    </nuxt-link>
                  </div>
                </div>
              </div>

              <div
                class="flex px-4 w-full sm:w-1/2 md:w-1/2 lg:w-1/2 xl:w-1/2 mx-auto"
              >
                <div>
                  <div class="max-w-sm rounded overflow-hidden cards">
                    <div class="font-bold text-lg mb-2 px-3 pt-5">
                      Privacy Policy
                    </div>
                    <div class="pb-5 px-3 text-sm">
                      This Privacy Policy tells you how we collect personal and
                      other information about...
                    </div>
                    <img
                      class="w-full mb-3"
                      src="~assets/policyIcons/secured-lock.png"
                      alt="secured lock card"
                    />
                    <nuxt-link
                      to="/privacy/terms-and-policies/privacy-policy"
                      class=""
                    >
                      <div class="float-left pl-5 pb-4 read-more">
                        READ MORE
                      </div>
                      <div class="float-right pb-4 pr-5 mt-1 mr-2">
                        <img src="~assets/right-arrow.png" alt="right-arrow" />
                      </div>
                    </nuxt-link>
                  </div>
                </div>
              </div>
            </div>

            <div class="md:flex mb-4">
              <div
                class="flex px-4 w-full sm:w-1/2 md:w-1/2 lg:w-1/2 xl:w-1/2 mx-auto"
                style="margin-bottom: 18px"
              >
                <div>
                  <div class="max-w-sm rounded overflow-hidden cards">
                    <div class="font-bold text-lg mb-2 px-3 pt-5">
                      Security Policy
                    </div>
                    <div class="pb-5 px-3 text-sm">
                      This security policy tells you the security measures put
                      in place by Scelloo...
                    </div>
                    <img
                      class="w-full mb-3"
                      src="~assets/policyIcons/padlock.png"
                      alt="security card"
                    />
                    <nuxt-link
                      to="/privacy/terms-and-policies/security-policy"
                      class=""
                    >
                      <div class="float-left pl-5 pb-4 read-more">
                        READ MORE
                      </div>
                      <div class="float-right pb-4 pr-5 mt-1 mr-2">
                        <img src="~assets/right-arrow.png" alt="right-arrow" />
                      </div>
                    </nuxt-link>
                  </div>
                </div>
              </div>
              <div
                class="flex px-4 w-full sm:w-1/2 md:w-1/2 lg:w-1/2 xl:w-1/2 mx-auto"
              >
                <div>
                  <div class="max-w-sm rounded overflow-hidden cards">
                    <div class="font-bold text-lg mb-2 px-3 pt-5">
                      Non-Disclosure Agreement
                    </div>
                    <div class="pb-5 px-3 text-sm">
                      THIS NON-DISCLOSURE AGREEMENT (the "Agreement”) is entered
                      into: By and...
                    </div>
                    <img
                      class="w-full mb-3"
                      src="~assets/policyIcons/folder.png"
                      alt="security card"
                    />
                    <nuxt-link
                      to="/privacy/terms-and-policies/non-disclosure-agreement"
                      class=""
                    >
                      <div class="float-left pl-5 pb-4 read-more">
                        READ MORE
                      </div>
                      <div class="float-right pb-4 pr-5 mt-1 mr-2">
                        <img src="~assets/right-arrow.png" alt="right-arrow" />
                      </div>
                    </nuxt-link>
                  </div>
                </div>
              </div>
            </div>
          </div>
        </div>
      </main>
    </div>
  </no-ssr>
</template>

<script>
import AppHeader from './../../../components/header/AppHeader'
export default {
  components: {
    AppHeader,
  },
}
</script>

<style scoped>
.cards {
  border: 1px solid #cfcfcf;
  border-radius: 6px;
}
.user-terms-of-use-container {
  background-color: #fbfbfb;
}
.read-more {
  color: #3598da;
}
* {
  color: #000;
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
  background-image: linear-gradient(269.56deg, #47c9fa 15.32%, #4881da 79.59%);
  background-repeat: no-repeat;
  background-size: 100% 100%;
  color: white;
}

@media (max-width: 480px) {
  .user-terms-of-services-cards {
    margin: auto;
  }
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
