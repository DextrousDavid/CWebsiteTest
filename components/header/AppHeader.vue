<template>
  <div>
    <nav
      class="flex-wrap justify-between nav-bg p-6"
      :class="fixed ? 'sticky' : null"
    >
      <div class="items-start flex-shrink-0 text-white mr-6 log-wrapper">
        <nuxt-link to="/">
          <img
            class="nav-image xl:mr-5 cloudenly-logo"
            src="/img/cloudenly-logo.svg"
          />
        </nuxt-link>
      </div>

      <div class="block lg:hidden" @click="toggle">
        <button
          type="button"
          class="flex items-center px-3 py-2 rounded text-black shadow-md hover:bg-gray-200 btnscoped"
        >
          <svg
            class="fill-current h-4 w-4"
            viewBox="0 0 20 20"
            xmlns="http://www.w3.org/2000/svg"
          >
            <title>Menu</title>
            <path d="M0 3h20v2H0V3zm0 6h20v2H0V9zm0 6h20v2H0v-2z" />
          </svg>
        </button>
      </div>
      <div
        :class="open ? 'block' : 'hidden'"
        class="w-full block flex-grow lg:flex lg:items-center lg:w-auto"
      >
        <div class="text-sm lg:flex-grow">
          <li
            class="list-item-navigation block mt-4 lg:inline-block lg:mt-0 hover:bg-gray-200 py-2 px-2 pt-1 rounded duration-300"
          >
            Products
          </li>

          <nuxt-link
            to="/pricing"
            class="list-item-navigation block mt-4 lg:inline-block lg:mt-0 hover:bg-gray-200 py-2 px-2 pt-1 rounded duration-300"
          >
            Pricing
          </nuxt-link>

          <li
            class="list-item-navigation block mt-4 lg:inline-block lg:mt-0 hover:bg-gray-200 py-2 px-2 pt-1 rounded duration-300"
          >
            Partners
          </li>
          <nuxt-link
            class="list-item-navigation block mt-4 lg:inline-block lg:mt-0 hover:bg-gray-200 py-2 px-2 pt-1 rounded duration-300"
            to="/resources"
          >
            Resources
          </nuxt-link>
          <li
            class="list-item-navigation block mt-4 lg:inline-block lg:mt-0 hover:bg-gray-200 py-2 px-2 pt-1 rounded duration-300"
          >
            Talk to an Expert
          </li>
        </div>
        <no-ssr>
          <div class="nav-item-left">
            <a
              href="http://dev-quantum-frontend.s3-website.eu-west-2.amazonaws.com/"
              class="sign-in-nav list-item-navigation block mt-4 lg:inline-block lg:mt-0 hover:bg-gray-200 py-2 px-2 pt-1 rounded duration-300"
            >
              Sign In
            </a>
            <!-- <nuxt-link
            to="/signup"
            class="join-btn inline-block text-sm px-6 py-4 leading-none border rounded text-white hover:bg-white hover:text-blue-700 mt-4 mr-4 lg:mt-0 shadow-md duration-200"
          >
            Sign Up
          </nuxt-link> -->
            <a
              href="http://dev-quantum-frontend.s3-website.eu-west-2.amazonaws.com/signup"
              class="join-btn inline-block text-sm px-6 py-4 leading-none border rounded text-white hover:bg-white hover:text-blue-700 mt-4 mr-4 lg:mt-0 shadow-md duration-200"
            >
              Sign Up
            </a>
          </div>
        </no-ssr>
      </div>
    </nav>
  </div>
</template>
<script>
export default {
  data() {
    return {
      open: false,
      fixed: false,
    }
  },
  beforeMount() {
    window.addEventListener('scroll', this.stickNavbar)
  },
  methods: {
    toggle() {
      this.open = !this.open
    },
    stickNavbar() {
      if (window.pageYOffset > 100) {
        //  console.log(pageYOffset, "see")
        this.fixed = true
      } else {
        this.fixed = false
      }
    },
  },
}
</script>
<style scoped>
.btnscoped {
  outline: none;
}

.sticky {
  position: fixed;
  width: 100%;
  /* background: #fff; */
  /* box-shadow: inset 0px -1px 0px #efefef; */
  z-index: 1;
  -webkit-transition: background 0.5s ease-in-out, padding 0.5s ease-in-out;
  -moz-transition: background 0.5s ease-in-out, padding 0.5s ease-in-out;
  transition: background 0.5s ease-in-out, padding 0.5s ease-in-out;
}
.nuxt-link-exact-active {
  color: #4781dc;
}

@media (min-width: 1280px) {
  .nav-image {
    /* margin-left: 3.2rem; */
  }
}
</style>
