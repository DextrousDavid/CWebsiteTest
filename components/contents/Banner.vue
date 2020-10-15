<template>
  <div>
    <section class="banner mb-8 pt-20">
      <div class="content-center mr-3 ml-3">
        <h1 class="font-normal">How can we help you?</h1>
        <div style="max-width: 550px; margin: auto">
          <p class="font-normal">Find help and learning resources below</p>
        </div>
      </div>
    </section>
  </div>
</template>

<script>
export default {
  name: 'Banner',
  components: {},
  head() {
    return {
      link: [
        {
          rel: 'stylesheet',
          href:
            '//db.onlinewebfonts.com/c/0007c768c0c6149485a44a0409d9433c?family=GalanoGrotesque-Regular',
        },
      ],
    }
  },
}
</script>

<style scoped>
h1,
* {
  font-family: GalanoGrotesque-Medium;
}
p,
a {
  margin: 0;
  padding: 0;
}
h1 {
  margin-top: -50px;
  padding: 10px 0;
  font-size: 36px;
  vertical-align: top;
}
p {
  font-size: 15px;
  text-align: center;
  margin: auto;
}

.banner {
  max-width: 100%;
  padding: 80px 0;
  text-align: center;
  background-image: url('rectangle3.jpg');
  background-repeat: no-repeat;
  background-size: 100% 100%;
  color: white;
}

@media (max-width: 728px) {
  p {
    font-size: 16px;
  }

  h1 {
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
