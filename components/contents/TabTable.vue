<template>
  <v-app class="tab-table">
    <v-card elevation="3">
      <template>
        <v-tabs centered light>
          <label>
            <v-tab>
              <input
                type="radio"
                class="form-radio radio-bg"
                name="radio"
                value="1"
                checked
              /><span style="margin-left: 4px">Monthly</span></v-tab
            >
          </label>
          <label>
            <v-tab>
              <input
                type="radio"
                class="form-radio text-indigo-600"
                name="radio"
                value="1"
              /><span style="margin-left: 4px">Annually</span>
            </v-tab>
          </label>
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
                    Billed Monthly<span class="float-right">N55,632</span>
                  </p>
                </v-card-text>
                <div class="my-2 d-flex justify-center">
                  <v-btn class="px-9" color="warning" dark>
                    Try for free
                  </v-btn>
                </div>
                <div class="my-2 d-flex justify-center">
                  <v-btn class="px-14" color="success" dark> Buy Now </v-btn>
                </div>
              </div>
            </v-card>
          </v-tab-item>
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
                  <v-btn class="px-9" color="warning" dark>
                    Try for free
                  </v-btn>
                </div>
                <div class="my-2 d-flex justify-center">
                  <v-btn class="px-14" color="success" dark> Buy Now </v-btn>
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
  .tab-table {
    margin-top: 4rem;
  }
}

@media (min-width: 1024px) {
  .tab-table {
    margin-top: 20rem;
  }
}

@media (min-width: 1024px) {
  .tab-table {
    margin-top: 9rem;
  }
}

@media (min-width: 1280px) {
  .tab-table {
    margin-top: -4rem;
  }
}
.v-tabs:not(.v-tabs--vertical) .v-tab {
  white-space: normal;
  margin-top: -6px;
  padding: 20px 15px;
}
/* @media (min-width: 1264px) {
  .tab-table {
    margin-top: -1rem;
  }
} */
</style>
