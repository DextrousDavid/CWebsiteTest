<template>
  <div>
    <Nuxt />
    <AppFooter />
  </div>
</template>
<script>
import AppFooter from '../components/footer/AppFooter'
export default {
  components: {
    AppFooter,
  },
  head() {
    return {
      title:
        'Cloudenly - Grow Your Business With Ease',
      meta: [
        {
          hid:
            'Cloudenly - Grow Your Business With Ease',
          name:
            'Cloudenly - Grow Your Business With Ease',
          content:
            'Cloudenly - Grow Your Business With Ease',
        },
      ],
    }
  },
}
</script>
<style>
@import '../assets/css/app.css';
@import '../assets/fonts/stylesheet.css';
/* @import 'bootstrap/dist/css/bootstrap.min.css'; */

* {
  font-family: GalanoGrotesque;
}

*,
*::before,
*::after {
  box-sizing: border-box;
  margin: 0;
}

.button--green {
  display: inline-block;
  border-radius: 4px;
  border: 1px solid #3b8070;
  color: #3b8070;
  text-decoration: none;
  padding: 10px 30px;
}

.button--green:hover {
  color: #fff;
  background-color: #3b8070;
}

.button--grey {
  display: inline-block;
  border-radius: 4px;
  border: 1px solid #35495e;
  color: #35495e;
  text-decoration: none;
  padding: 10px 30px;
  margin-left: 15px;
}

.button--grey:hover {
  color: #fff;
  background-color: #35495e;
}
</style>
