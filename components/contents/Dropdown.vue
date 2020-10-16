<template>
  <div class="relative">
    <button
      class="block overflow-hidden focus:outline-none focus:border-white"
      @click="isOpen = !isOpen"
    >
      More
      <!-- Heroicon name: chevron-down -->

      <i class="fa fa-ellipsis-v fa-sm"></i>

      <!-- <i class="fa fa-search fa-md" aria-hidden="true"></i> -->
    </button>
    <div
      v-if="isOpen"
      class="absolute mt-2 py-2 w-40 bg-white rounded-lg shadow-xl transition duration-500 ease-in-out"
      @click="isOpen = !isOpen"
    >
      <a
        href="#"
        class="block px-2 py-2 text-gray-800 hover:bg-indigo-500 hover:text-white transition duration-150 ease-in-out"
        >Developer Documentation
      </a>
      <a
        href="#"
        class="block px-2 py-2 text-gray-800 hover:bg-indigo-500 hover:text-white transition duration-150 ease-in-out"
        >Developer Documentation 2
      </a>
      <a
        href="#"
        class="block px-2 py-2 text-gray-800 hover:bg-indigo-500 hover:text-white transition duration-300 ease-in-out"
        >Developer Documentation 3</a
      >
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      isOpen: false,
    }
  },
}
</script>

<style scoped>
i {
  color: rgb(59, 178, 226);
  padding-left: 10px;
  margin-left: -9px;
}
</style>
