/* eslint-disable */
<template>
  <div>
    <div class="sm:flex product-wrapper">
      <!-- :items-to-slide="3" -->
      <hooper :items-to-show="3">
        <slide> slide 1 </slide>
        <slide> slide 2 </slide>
        <slide> slide 3 </slide>
        <slide> slide 4 </slide>
        <slide> slide 5 </slide>
        <slide> slide 6 </slide>
        <hooper-navigation slot="hooper-addons"></hooper-navigation>
        <hooper-pagination slot="hooper-addons"></hooper-pagination>
      </hooper>
    </div>
  </div>
</template>
<script>
import { Hooper, Slide, Navigation as HooperNavigation } from 'hooper'
import 'hooper/dist/hooper.css'
export default {
  components: {
    Hooper,
    Slide,
    HooperNavigation,
  },
  data() {
    return {}
  },
}
</script>
<style scoped>
/* Product Card */
.product-wrapper {
  background-color: rgb(241, 245, 251, 0.4);
  border: 5px solid #ffffff;
  border-radius: 15px;
  margin-top: 30px;
  width: 1304px;
  /* height: 792px; */
  padding: 150px 80px;
  position: relative;
}
</style>

<style></style>
