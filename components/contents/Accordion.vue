<template>
  <no-ssr>
    <div style="position: relative" class="mt-3">
      <v-app>
        <div class="xs:mx-2 sm:mx-2 md:mx-48 lg:mx-56">
          <v-expansion-panels style="z-index: 0" accordion hover>
            <v-expansion-panel
              v-for="userGuide in userGuides"
              :key="userGuide.id"
            >
              <v-expansion-panel-header>
                {{ userGuide.heading }}
                <template v-slot:actions>
                  <v-icon color="primary">$expand</v-icon>
                </template>
              </v-expansion-panel-header>

              <v-expansion-panel-content color="blue lighten-5">
                <a :href="userGuide.url1">
                  <div class="divtextColor mt-2">
                    {{ userGuide.content1 }}
                  </div>
                </a>

                <a :href="userGuide.url2">
                  <div class="divtextColor mt-2">
                    {{ userGuide.content2 }}
                  </div>
                </a>

                <a :href="userGuide.url3">
                  <div class="divtextColor mt-2">
                    {{ userGuide.content3 }}
                  </div>
                </a>

                <a :href="userGuide.url4">
                  <div class="divtextColor mt-2">
                    {{ userGuide.content4 }}
                  </div>
                </a>

                <a :href="userGuide.url5">
                  <div class="divtextColor mt-2">
                    {{ userGuide.content5 }}
                  </div>
                </a>

                <a :href="userGuide.url6">
                  <div class="divtextColor mt-2">
                    {{ userGuide.content6 }}
                  </div>
                </a>

                <a target="_blank" :href="userGuide.url7">
                  <div class="divtextColor mt-2">
                    {{ userGuide.content7 }}
                  </div>
                </a>

                <a :href="userGuide.url8">
                  <div class="divtextColor mt-2">
                    {{ userGuide.content8 }}
                  </div>
                </a>

                <a :href="userGuide.url9">
                  <div class="divtextColor mt-2">
                    {{ userGuide.content9 }}
                  </div>
                </a>
              </v-expansion-panel-content>
            </v-expansion-panel>
          </v-expansion-panels>
        </div>
      </v-app>
    </div>
  </no-ssr>
</template>

<script>
export default {
  components: {},
  props: {
    userGuides: {
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

<style>
.v-expansion-panels {
  border-radius: 4px;
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
  list-style-type: none;
  padding: 0;
  width: 100%;
  /* z-index: 1; */
}
* {
  font-family: GalanoGrotesque-Medium;
  color: #828282;
}
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
.divtextColor:hover {
  color: #0069bebd;
}
</style>
