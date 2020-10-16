<template>
  <div class="flex flex-wrap px-12 justify-center bg-gray-200 p-6 footer">
    <div class="flex flex-wrap mb-3 text-center w-full">
      <hr class="sm:invisible" />
      <div
        class="w-full sm:w-1/2 sm:text-center md:text-left md:w-1/4 lg:w-1/5 pl:w-1/5-8 mb-6 px-2"
      >
        <div class="menu-head">Products</div>
        <div class="list-element">Optima</div>
        <div class="list-element">HumanaR</div>
        <div class="list-element">Dome</div>
        <div class="list-element">Quantum</div>
        <div class="list-element">Ally</div>
        <!-- <div class="list-element">Quantum</div> -->
      </div>
      <div
        class="w-full sm:w-1/2 sm:text-center md:text-left md:w-1/4 lg:w-1/5 pl:w-1/5-8 mb-6 px-2"
      >
        <div class="menu-head">Pricing</div>
        <div class="list-element">Optima</div>
        <div class="list-element">HumanaR</div>
      </div>

      <div
        class="w-full sm:w-1/2 sm:text-center md:text-left md:w-1/4 lg:w-1/5 pl:w-1/5-8 mb-6 px-2"
      >
        <div class="menu-head">Partners</div>
        <div class="list-element">Find a Partner</div>
        <div class="list-element">Become a Partner</div>
      </div>

      <div
        class="w-full sm:w-1/2 sm:text-center md:text-left md:w-1/4 lg:w-1/5 pl:w-1/5-8 mb-6 px-2"
      >
        <div class="menu-head">Resources</div>
        <div class="list-element">Product Overview</div>
        <div class="list-element">FAQ</div>
        <div class="list-element">User Guide</div>
        <div class="list-element">Blogs / Events</div>
        <div class="list-element">Community</div>
        <div class="list-element">Developer Documentation</div>
        <div class="list-element">Academy</div>
        <div class="list-element">Demo</div>
      </div>

      <div
        class="w-full sm:w-1/2 sm:text-center md:text-left md:w-2/4 lg:w-1/5 pl:w-1/5-8 mb-6 px-2"
      >
        <div class="menu-head">Support</div>
        <div class="list-element">Support@cloudenly.com</div>
        <a href="tel:+2348159530070">
          <div class="list-element">+234 8159530070</div>
        </a>
        <a href="tel:+234556655667">
          <div class="list-element">+234 5566 55667</div>
        </a>
      </div>

      <hr style="margin-top: 17px; border-top-color: #e1e0e0" />

      <div class="flex flex-wrap mb-3 w-full md:text-left">
        <div class="w-full mb-6 px-2">
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

      <div
        class="flex flex-wrap mb-3 w-full -mt-3 xs:-px-8 sm:-px-8 md:px-2 lg:px-2"
      >
        <div class="w-full md:w-2/4 lg:w-3/4 mb-3 text-left">
          <div class="sm:flex bottom-navigation-div">
            <div class="bottom-link">Terms of Service</div>
            <div class="bottom-link">Privacy Information</div>
            <div class="bottom-link">Security</div>
            <div class="bottom-link">Careers</div>
            <div class="bottom-link">Contract</div>
          </div>
          <div class="text-newsletter mt-1">
            <p class="text-newsletter">
              Scelloo HQ, Plot 16 New Creation Street, Lekki, Lagos, Nigeria.
            </p>
            <p class="text-newsletter copyright-margin-bottom md:mt-1">
              &copy; Copyright 2020 Scelloo Nigeria. All Rights Reserved.
            </p>
          </div>
        </div>

        <div class="w-full md:w-2/4 lg:w-1/4 mb-3 text-left">
          <div class="newsleter-head">Suscribe to our Newsletter</div>
          <div class="text-newsletter">
            Subscribe to our newsletters. We don’t Bite!
          </div>
          <form class="mt-1" action="#">
            <div class="flex items-center mb-6">
              <input
                id="inline-full-name"
                class="bg-gray-200 appearance-none border-2 border-gray-200 w-full font-extrabold py-2 px-2 text-black leading-tight focus:outline-none hover:border-blue-500 focus:bg-white focus:border-blue-500"
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
          </form>
        </div>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  data() {
    return {}
  },
  methods: {},
}
</script>
<style scoped>
.footer {
  margin-top: 6em;
}

a {
  color: #000;
}
li {
  padding-top: 5px;
}
a:hover {
  color: #ddd;
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

  .footer {
    margin-top: 5em;
  }
}
.copyright-margin-bottom {
  margin-bottom: 2px;
}
</style>
