<template>
  <div>
    <TryCloudenlyForFree />
    <div class="bg-white pb-8" style="font-size: 15px">
      <div
        class="flex flex-wrap px-12 justify-center p-6 pt-12 app-footer leading-7"
      >
        <div class="flex flex-wrap mb-3 text-center w-full">
          <!-- <hr class="sm:invisible" /> -->
          <!-- Products to support begins here -->
          <div class="flex flex-wrap text-center w-full lg:mb-1">
            <!-- Cloudenly logo and social icons goes in here -->
            <div
              class="w-full sm:w-1/2 sm:text-center md:text-left md:w-1/4 lg:w-1/6 pl:w-1/5-8 px-2 xl:mr-48"
            >
              <div class="w-full mb-6 px-2">
                <div class="xs:text-center md:text-left">
                  <div class="inline-block">
                    <nuxt-link to="/">
                      <img
                        class="footer-logo"
                        src="img/Cloudenly-logo-width.svg"
                        alt="cloudenly logo"
                      />
                    </nuxt-link>
                  </div>
                </div>
                <div class="xs:text-center md:text-left mt-4">
                  <div class="inline-block mr-2">
                    <img src="/img/whatsapp-icon.svg" />
                  </div>
                  <div class="inline-block mr-2">
                    <img src="/img/twitter-icon.svg" />
                  </div>
                  <div class="inline-block mr-2">
                    <img src="/img/facebook-icon.svg" />
                  </div>
                  <div class="inline-block mr-2">
                    <img src="/img/instagram-icon.svg" />
                  </div>
                </div>
              </div>
            </div>

            <div
              class="w-full sm:w-1/2 sm:text-center md:text-left md:w-1/4 lg:w-1/6 pl:w-1/5-8 mb-6 px-2"
            >
              <div class="menu-head">Products</div>
              <div class="list-element">Optima</div>
              <div class="list-element">HumanaR</div>
              <div class="list-element">
                Dome <span style="font-size: 10px">(coming soon)</span>
              </div>
              <!-- <div class="list-element">Quantum</div>
              <div class="list-element">Ally</div> -->
              <!-- <div class="list-element">Quantum</div> -->
            </div>
            <div
              class="w-full sm:w-1/2 sm:text-center md:text-left md:w-1/4 lg:w-1/6 mb-6 px-2 xl:-mx-20"
            >
              <nuxt-link to="/pricing" class="menu-head hover:underline"
                >Pricing</nuxt-link
              >
              <div class="list-element">Optima</div>
              <div class="list-element">HumanaR</div>
            </div>

            <div
              class="w-full sm:w-1/2 sm:text-center md:text-left md:w-1/4 lg:w-1/6 mb-6 px-2"
            >
              <div class="menu-head">Partners</div>
              <div class="list-element">Find a Partner</div>
              <no-ssr>
                <a href="https://scelloo.com/partnership/" target="_blank">
                  <div class="list-element hover:underline">
                    Become a Partner
                  </div>
                </a>
              </no-ssr>
            </div>

            <div
              class="w-full sm:w-1/2 sm:text-center md:text-left md:w-1/4 lg:w-1/6 mb-6 px-2 xl:-mx-6"
            >
              <nuxt-link to="/resources">
                <div class="menu-head hover:underline">
                  Resources
                </div></nuxt-link
              >
              <nuxt-link to="/resources/product-overview">
                <div class="list-element hover:underline">Product Overview</div>
              </nuxt-link>
              <nuxt-link to="/faq"
                ><div class="list-element hover:underline">FAQ</div></nuxt-link
              >
              <nuxt-link to="/resources/userguide">
                <div class="list-element hover:underline">User Guide</div>
              </nuxt-link>
              <div class="list-element">Blogs</div>
              <div class="list-element">Events</div>
              <div class="list-element">Community</div>
              <div class="list-element">Developer Documentation</div>
              <div class="list-element">Academy</div>
              <div class="list-element">Demo</div>
            </div>

            <div
              class="w-full sm:w-1/2 sm:text-center md:text-left md:w-2/4 lg:w-1/6 px-2"
            >
              <div to="/support" class="menu-head">Support</div>
              <div class="list-element">support@cloudenly.com</div>
              <a href="tel:+2349060020838">
                <div class="list-element hover:underline">09060020838</div>
              </a>
              <a href="tel:+2349060071225">
                <div class="list-element hover:underline">09060071225</div>
              </a>
              <nuxt-link to="/support"
                ><div class="list-element hover:underline">
                  Get Help
                </div></nuxt-link
              >
            </div>

            <!-- <hr style="margin-top: 17px; border-top-color: red" /> -->

            <!-- <div class="flex flex-wrap mb-3 w-full md:text-left">
          <div class="w-full mb-2 px-2">
            <div>
              <img src="~assets/cloudenly-logo.svg" />
            </div>
            <div class="inline-block mr-2">
              Icons starts
              <img src="/img/whatsapp-icon.svg" />
            </div>
            <div class="inline-block mr-2">
              <img src="/img/twitter-icon.svg" />
            </div>
            <div class="inline-block mr-2">
              <img src="/img/facebook-icon.svg" />
            </div>
            <div class="inline-block mr-2">
              <img src="/img/instagram-icon.svg" />
              icon ends
            </div>
          </div>
        </div> -->
          </div>
        </div>
      </div>

      <hr class="w-full" style="border: 1px solid #e1e0e0" />

      <!-- Product to support ends here -->

      <!-- Terms of service div begins here -->
      <div class="flex flex-wrap px-12 justify-center mt-4">
        <div
          class="flex flex-wrap mb-3 mt-2 w-full xs:-px-8 sm:-px-8 md:px-2 lg:px-2 -mx-2"
        >
          <div class="w-full md:w-3/4 lg:w-3/4 mb-3 text-left px-2 sm:mt-3">
            <div class="sm:flex bottom-navigation-div">
              <nuxt-link to="/privacy/terms-and-policies">
                <!-- <div class="bottom-link">Terms of Service</div> -->

                <div class="bottom-link">Terms and Policies</div>
              </nuxt-link>

              <div class="bottom-link">Careers</div>
            </div>
            <div class="text-newsletter mt-2">
              <p class="text-newsletter">
                &copy; Copyright 2020 Scelloo Nigeria. All Rights Reserved.
                Scelloo HQ, Plot 16 New Creation Street, Lekki, Lagos, Nigeria.
              </p>
            </div>
          </div>

          <div class="w-full md:w-1/4 lg:w-1/4 mb-3 text-left px-2">
            <div class="newsleter-head">Suscribe to our Newsletter</div>
            <div class="text-newsletter" style="margin-bottom: 8px">
              Subscribe to our newsletters. We don’t Bite!
            </div>
            <!-- <form class="mt-1" action="#">
            <div class="flex items-center mb-6">
              <input
                id="inline-full-name"
                class="bg-gray-200 border-2 border-gray-200 w-full font-extrabold py-2 px-2 text-black leading-tight focus:outline-none hover:border-blue-500 focus:bg-white focus:border-blue-500"
                type="email"
                placeholder="Enter Email"
              />
              <button
                class="bg-blue-500 ml-2 hover:bg-white hover:text-blue-500 text-white font-extrabold py-2 px-2 shadow-lg duration-200 border rounded"
                type="submit"
              >
                Submit
              </button>
            </div>
          </form> -->
            <form class="w-full max-w-sm">
              <div
                class="flex items-center border py-2 focus:shadow-outline pr-3"
              >
                <input
                  class="appearance-none bg-transparent border w-full rounded text-gray-700 py-1 px-1 leading-tight focus:outline-none"
                  type="text"
                  placeholder="Enter Email"
                  aria-label="Enter Email"
                />
                <button>
                  <img
                    class="fill-current h-6 w-6"
                    src="~assets/arrow-button.svg"
                    alt="cloudenly logo"
                  />
                </button>
              </div>
            </form>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>
<script>
import TryCloudenlyForFree from '../contents/TryCloudenlyForFree'
export default {
  components: {
    TryCloudenlyForFree,
  },
  data() {
    return {}
  },
  methods: {},
}
</script>
<style scoped>
.footer-logo {
  width: 68px;
}
/* .app-footer {
  margin-top: 6em;
} */

a {
  color: #000;
}
li {
  padding-top: 5px;
}
a:hover {
  color: #080101;
}

button {
  color: #fff;
}

@media (max-width: 642px) {
  .bottom {
    text-align: center;
  }
  .pl-8 {
    padding-left: 0px;
  }

  /* .app-footer {
    margin-top: 5em;
  } */
}
.copyright-margin-bottom {
  margin-bottom: 2px;
}
.list-element {
  font-size: 14px;
}
</style>
