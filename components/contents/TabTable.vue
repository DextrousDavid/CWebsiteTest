<template>
  <v-app>
    <v-card elevation="3">
      <template>
        <v-tabs centered>
          <v-tab> Annually </v-tab>
          <v-tab>Monthly</v-tab>
          <v-tab-item>
            <v-card flat>
              <v-card-text class="grey lighten-3">
                10 Users<span class="float-right">N80</span>
              </v-card-text>

              <v-card-text class="grey lighten-5">
                User Discount<span class="float-right">_ _ _</span>
              </v-card-text>

              <v-card-text class="grey lighten-3">
                9 Apps<span class="float-right">4800</span>
              </v-card-text>

              <v-card-text class="grey lighten-5">
                App Discount<span class="float-right">_ _ _</span>
              </v-card-text>

              <v-card-text class="grey lighten-3">
                Total / Month<span class="float-right">N4,632</span>
              </v-card-text>

              <div class="grey lighten-5">
                <v-card-text
                  ><p class="font-weight-thin">
                    Billed Annually<span class="float-right">N55,632</span>
                  </p>
                </v-card-text>
                <div class="my-2 d-flex justify-center">
                  <v-btn class="px-8" color="warning" dark>
                    Try it for free
                  </v-btn>
                </div>
                <div class="my-2 d-flex justify-center">
                  <v-btn class="px-15" color="success" dark> Buy Now </v-btn>
                </div>
              </div>
            </v-card>
          </v-tab-item>
          <v-tab-item>
            <v-card flat>
              <v-card-text class="grey lighten-3">
                Cloudenly<span class="float-right">Cloudenly</span>
              </v-card-text>

              <v-card-text class="grey lighten-5">
                Cloudenly<span class="float-right"> Cloudenly</span>
              </v-card-text>

              <v-card-text class="grey lighten-3"
                >Cloudenly<span class="float-right">Cloudenly</span>
              </v-card-text>

              <v-card-text class="grey lighten-5">
                Cloudenly<span class="float-right">Cloudenly</span>
              </v-card-text>

              <v-card-text class="grey lighten-3">
                Cloudenly<span class="float-right">Cloudenly</span>
              </v-card-text>

              <div class="grey lighten-5">
                <v-card-text
                  ><p class="font-weight-thin">
                    Cloudenly<span class="float-right">Cloudenly</span>
                  </p>
                </v-card-text>
                <div class="my-2 d-flex justify-center">
                  <v-btn class="px-8" color="warning" dark>
                    Try it for free
                  </v-btn>
                </div>
                <div class="my-2 d-flex justify-center">
                  <v-btn class="px-15" color="success" dark> Buy Now </v-btn>
                </div>
              </div>
            </v-card>
          </v-tab-item>
        </v-tabs>
      </template>
    </v-card>
  </v-app>
</template>

<script>
export default {
  name: 'TabTable',
  data() {
    return {}
  },
}
</script>

<style scoped>
* {
  font-family: GalanoGrotesque-Medium;
  /* color: #828282; */
}

@media (min-width: 960px) {
  .col-md-4 {
    flex: 0 0 33.3333333333%;
    max-width: 33.3333333333%;
    margin-top: 100px;
  }
}
</style>
