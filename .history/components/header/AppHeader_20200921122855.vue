<template>
  <div>
    <nav
      class="flex  flex-wrap nav-bg p-6"
      :class="fixed ? 'sticky' : null"
    >
      <div class="flex items-center flex-shrink-0 text-white mr-6 log-wrapper">
        <img src="/img/cloudenly-logo.svg" />
      </div>
      <div class="block lg:hidden">
        <button
          class="flex items-center bg-indigo-600 px-3 py-2 border rounded text-teal-200 border-teal-400 hover:text-white hover:border-white"
          @click="toggle"
        >
          <svg
            class="fill-current h-3 w-3"
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
          <li class="list-item-navigation block mt-4 lg:inline-block lg:mt-0">
            Products
          </li>
          <li class="list-item-navigation block mt-4 lg:inline-block lg:mt-0">
            Pricing
          </li>
          <li class="list-item-navigation block mt-4 lg:inline-block lg:mt-0">
            Partners
          </li>
          <li class="list-item-navigation block mt-4 lg:inline-block lg:mt-0">
            Resources
          </li>
          <li class="list-item-navigation block mt-4 lg:inline-block lg:mt-0">
            Talk to an Expert
          </li>
        </div>
        <div>
          <li
            class="sign-in-nav list-item-navigation block mt-4 lg:inline-block lg:mt-0"
          >
            Sign In
          </li>
          <a
            href="#"
            class="join-btn inline-block text-sm px-4 py-2 mt-4 lg:mt-0"
          >
            Join us Now
          </a>
        </div>
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
</style>
