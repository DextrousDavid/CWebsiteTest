/* eslint-disable prettier/prettier */
<template>
  <div>
    <nav class="flex-wrap justify-between nav-bg p-8 mb-20">
      <div class="items-center flex-shrink-0 text-white mr-6 log-wrapper">
        <nuxt-link to="/">
          <img
            class="xl:ml-16 xl:mr-5 cloudenly-logo"
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
          <nuxt-link
            to="/resources/product-overview"
            class="list-item-navigation block mt-4 lg:inline-block lg:mt-0 hover:bg-gray-200 py-2 px-2 pt-1 rounded duration-300"
          >
            Product Overview
          </nuxt-link>
          <nuxt-link
            to="/resources/userguide"
            class="list-item-navigation block mt-4 lg:inline-block lg:mt-0 text-blue-500 hover:bg-gray-200 py-2 pt-1 px-2 rounded userguide duration-300"
          >
            User Guide
          </nuxt-link>
          <li
            class="list-item-navigation block mt-4 lg:inline-block lg:mt-0 hover:bg-gray-200 py-2 px-2 pt-1 rounded duration-300"
          >
            Blogs
          </li>
          <li
            class="list-item-navigation block mt-4 lg:inline-block lg:mt-0 hover:bg-gray-200 py-2 px-2 pt-1 rounded duration-300"
          >
            Events
          </li>
          <nuxt-link to="">
            <li
              class="list-item-navigation block mt-4 lg:inline-block lg:mt-0 hover:bg-gray-200 py-2 px-2 pt-1 rounded duration-300"
            >
              Community
            </li></nuxt-link
          >

          <li
            class="list-item-navigation block mt-4 lg:inline-block lg:mt-0 hover:bg-gray-200 py-2 px-2 pt-1 rounded duration-300"
          >
            Developer Documentation
          </li>

          <li
            class="list-item-navigation block mt-4 lg:inline-block lg:mt-0 hover:bg-gray-200 py-2 px-2 pt-1 rounded duration-300"
          >
            Demo
          </li>
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
      fixed: true,
    }
  },
  //   Sticky
  //   beforeMount() {
  //     window.addEventListener('scroll', this.stickNavbar)
  //   },
  methods: {
    toggle() {
      this.open = !this.open
    },
    // stickNavbar() {
    //   if (window.pageYOffset > 100) {
    //     //  console.log(pageYOffset, "see")
    //     this.fixed = true
    //   } else {
    //     this.fixed = false
    //   }
    // },
  },
}
</script>
<style scoped>
.btnscoped {
  outline: none;
}

.userguide {
  color: #1034a6;
}

/* .sticky {
  position: fixed;
  width: 100%;

  z-index: 1;
  -webkit-transition: background 0.5s ease-in-out, padding 0.5s ease-in-out;
  -moz-transition: background 0.5s ease-in-out, padding 0.5s ease-in-out;
  transition: background 0.5s ease-in-out, padding 0.5s ease-in-out;
} */
</style>
