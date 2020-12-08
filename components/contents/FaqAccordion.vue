<template>
  <no-ssr>
    <div class="mb-4">
      <v-app>
        <!-- <v-container mx-16> -->
        <div>
          <v-expansion-panels style="z-index: 0" accordion hover>
            <v-expansion-panel v-for="faq in faqs" :key="faq.id">
              <v-expansion-panel-header>
                <span style="color: #2865ef">{{ faq.heading }}</span>
                <template v-slot:actions>
                  <v-icon color="primary">$expand</v-icon>
                </template>
              </v-expansion-panel-header>

              <v-expansion-panel-content color="white">
                <a :href="faq.url1">
                  <div class="divtextColor mt-2">
                    {{ faq.content1 }}
                  </div>
                </a>

                <a :href="faq.url2">
                  <div class="divtextColor mt-2">
                    {{ faq.content2 }}
                  </div>
                </a>

                <a :href="faq.url3">
                  <div class="divtextColor mt-2">
                    {{ faq.content3 }}
                  </div>
                </a>

                <a :href="faq.url4">
                  <div class="divtextColor mt-2">
                    {{ faq.content4 }}
                  </div>
                </a>

                <a :href="faq.url5">
                  <div class="divtextColor mt-2">
                    {{ faq.content5 }}
                  </div>
                </a>

                <a :href="faq.url6">
                  <div class="divtextColor mt-2">
                    {{ faq.content6 }}
                  </div>
                </a>

                <a :href="faq.url7">
                  <div class="divtextColor mt-2">
                    {{ faq.content7 }}
                  </div>
                </a>

                <a :href="faq.url8">
                  <div class="divtextColor mt-2">
                    {{ faq.content8 }}
                  </div>
                </a>

                <a :href="faq.url9">
                  <div class="divtextColor mt-2">
                    {{ faq.content9 }}
                  </div>
                </a>
              </v-expansion-panel-content>
            </v-expansion-panel>
          </v-expansion-panels>
        </div>
        <!-- </v-container> -->
      </v-app>
    </div>
  </no-ssr>
</template>

<script>
export default {
  components: {},
  props: {
    faqs: {
      type: Array,
      required: true,
    },
  },
  // fetch({ store }) {
  //   return axios
  //     .get('https://resources.cloudenly.com/wp-json/wp/v2/ht_kb/')
  //     .then((res) => {
  //       store.commit('frontPagePosts', res.data)
  //     })
  // },
  data() {
    return {}
  },
  // computed: {
  //   posts() {
  //     return this.$store.state.posts
  //   },
  // },
}
</script>

<style>
.v-expansion-panel::before {
  outline: none !important;
}

.v-expansion-panel-header {
  outline: none !important;
  font-weight: 550;
}

a {
  font-size: 15px;
}
.v-application--wrap {
  min-height: 1px !important;
}
.divtextColor {
  color: #000;
}
.divtextColor:visited {
  color: purple;
}
/* .divtextColor:hover {
  color: #0069bebd;
} */
</style>
