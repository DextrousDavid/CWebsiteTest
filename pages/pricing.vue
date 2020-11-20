<template>
  <no-ssr>
    <div>
      <AppHeader />
      <v-app>
        <section class="banner">
          <div class="content-center mr-3 ml-3">
            <h1 class="banner-h1 font-bold">Cloudenly Pricing</h1>
            <div style="max-width: 550px; margin: auto">
              <p class="banner-p font-normal">
                Flexible pricing options, from personal projects to enterprise
                applications, and everything in between
              </p>
            </div>
          </div>
        </section>
        <PricingTabs />
        <v-container>
          <div class="mt-16">
            <h3 class="mb-4">Choose the number of users</h3>
            <div>
              <div class="d-flex">
                <v-col cols="3" sm="2" md="1">
                  <v-text-field
                    id="input-20"
                    v-model="users"
                    min="1"
                    type="number"
                    required="required"
                    outlined
                  ></v-text-field>
                </v-col>
                <v-col cols="3" sm="2" md="1">
                  <v-btn
                    class="text-capitalize -ml-8"
                    color="primary"
                    style="
                      cursor: not-allowed;
                      pointer-events: none;
                      padding: 28px 15px;
                    "
                    >Users</v-btn
                  >
                </v-col>
                <v-col cols="5" sm="5" md="5">
                  <span class="ml-4">N80/user/ Month</span>
                </v-col>
              </div>
            </div>
          </div>

          <!-- Choose your apps starts here -->
          <div>
            <div>
              <v-row>
                <v-col class="lg:mt-20" cols="12" sm="12" md="8" lg="8">
                  <div class="mt-5">
                    <h3 class="mt-4 mb-2">Choose your apps</h3>
                  </div>
                  <v-row>
                    <v-col cols="12" sm="6" md="6" lg="4">
                      <v-card
                        max-width="auto"
                        max-height="80"
                        outlined
                        hover
                        color="grey lighten-4"
                      >
                        <!-- @click="append('640')" -->
                        <v-list-item three-line>
                          <v-list-item-avatar tile size="40">
                            <img src="~assets/apps/crm.png" alt="crm icon" />
                          </v-list-item-avatar>

                          <v-list-item-content
                            style="margin-top: -20px"
                            class="text-capitalize"
                          >
                            CRM
                            <v-list-item-subtitle style="margin-top: -34px"
                              >640/ Month</v-list-item-subtitle
                            >
                          </v-list-item-content>
                          <v-tooltip class="d-flex align-end" top>
                            <template v-slot:activator="{ on, attrs }">
                              <v-btn icon v-bind="attrs" v-on="on">
                                <v-icon small color="grey lighten-1">
                                  mdi-information
                                </v-icon>
                              </v-btn>
                            </template>
                            <span class="tooltip-notification"
                              >CRM. Learn More...</span
                            >
                          </v-tooltip>
                        </v-list-item>
                      </v-card>
                    </v-col>

                    <v-col cols="12" sm="6" md="6" lg="4">
                      <v-card
                        max-width="auto"
                        max-height="80"
                        flat
                        link
                        color="grey lighten-4"
                        style="border: 2px solid red"
                      >
                        <!-- @click="append('640')" -->
                        <!-- hover -->
                        <v-list-item three-line>
                          <v-list-item-avatar tile size="40">
                            <img
                              src="~assets/apps/purchase.png"
                              alt="purchase icon"
                            />
                          </v-list-item-avatar>

                          <v-list-item-content
                            style="margin-top: -20px"
                            class="text-capitalize"
                          >
                            Purchase
                            <v-list-item-subtitle style="margin-top: -34px"
                              >640/ Month</v-list-item-subtitle
                            >
                          </v-list-item-content>
                          <v-tooltip class="d-flex align-end" top>
                            <template v-slot:activator="{ on, attrs }">
                              <v-btn icon v-bind="attrs" v-on="on">
                                <v-icon small color="grey lighten-1">
                                  mdi-information
                                </v-icon>
                              </v-btn>
                            </template>
                            <span class="tooltip-notification"
                              >Purchase. Learn More...</span
                            >
                          </v-tooltip>
                        </v-list-item>
                      </v-card>
                    </v-col>

                    <v-col cols="12" sm="6" md="6" lg="4">
                      <v-card
                        max-width="auto"
                        max-height="80"
                        outlined
                        hover
                        color="grey lighten-4"
                      >
                        <v-list-item three-line>
                          <v-list-item-avatar tile size="40">
                            <img
                              src="~assets/apps/sales.png"
                              alt="sales icon"
                            />
                          </v-list-item-avatar>

                          <v-list-item-content
                            style="margin-top: -20px"
                            class="text-capitalize"
                            >Sales

                            <v-list-item-subtitle style="margin-top: -34px"
                              >640/ Month</v-list-item-subtitle
                            >
                          </v-list-item-content>
                          <v-tooltip class="d-flex align-end" top>
                            <template v-slot:activator="{ on, attrs }">
                              <v-btn icon v-bind="attrs" v-on="on">
                                <v-icon small color="grey lighten-1">
                                  mdi-information
                                </v-icon>
                              </v-btn>
                            </template>
                            <span class="tooltip-notification"
                              >Sales. Learn More...</span
                            >
                          </v-tooltip>
                        </v-list-item>
                      </v-card>
                    </v-col>

                    <v-col cols="12" sm="6" md="6" lg="4">
                      <v-card
                        max-width="auto"
                        max-height="80"
                        outlined
                        hover
                        color="grey lighten-4"
                      >
                        <v-list-item three-line>
                          <v-list-item-avatar tile size="40">
                            <img
                              src="~assets/apps/inventory.png"
                              alt="inventory icon"
                            />
                          </v-list-item-avatar>

                          <v-list-item-content
                            style="margin-top: -20px"
                            class="text-capitalize"
                          >
                            Inventory
                            <v-list-item-subtitle style="margin-top: -34px"
                              >640/ Month</v-list-item-subtitle
                            >
                          </v-list-item-content>
                          <v-tooltip class="d-flex align-end" top>
                            <template v-slot:activator="{ on, attrs }">
                              <v-btn icon v-bind="attrs" v-on="on">
                                <v-icon small color="grey lighten-1">
                                  mdi-information
                                </v-icon>
                              </v-btn>
                            </template>
                            <span class="tooltip-notification"
                              >Inventory. Learn More...</span
                            >
                          </v-tooltip>
                        </v-list-item>
                      </v-card>
                    </v-col>
                    <v-col cols="12" sm="6" md="6" lg="4">
                      <v-card
                        max-width="auto"
                        max-height="80"
                        outlined
                        hover
                        color="grey lighten-4"
                      >
                        <v-list-item three-line>
                          <v-list-item-avatar tile size="40">
                            <img
                              src="~assets/apps/payments.png"
                              alt="payments icon"
                            />
                          </v-list-item-avatar>

                          <v-list-item-content
                            style="margin-top: -20px"
                            class="text-capitalize"
                          >
                            Payments
                            <v-list-item-subtitle style="margin-top: -34px"
                              >640/ Month</v-list-item-subtitle
                            >
                          </v-list-item-content>
                          <v-tooltip class="d-flex align-end" top>
                            <template v-slot:activator="{ on, attrs }">
                              <v-btn icon v-bind="attrs" v-on="on">
                                <v-icon small color="grey lighten-1">
                                  mdi-information
                                </v-icon>
                              </v-btn>
                            </template>
                            <span class="tooltip-notification"
                              >Payments. Learn More...</span
                            >
                          </v-tooltip>
                        </v-list-item>
                      </v-card>
                    </v-col>

                    <v-col cols="12" sm="6" md="6" lg="4">
                      <v-card
                        max-width="auto"
                        max-height="80"
                        outlined
                        hover
                        color="grey lighten-4"
                      >
                        <v-list-item three-line>
                          <v-list-item-avatar tile size="40">
                            <img
                              src="~assets/apps/accounts.png"
                              alt="accounts icon"
                            />
                          </v-list-item-avatar>

                          <v-list-item-content
                            style="margin-top: -20px"
                            class="text-capitalize"
                          >
                            Accounting
                            <v-list-item-subtitle style="margin-top: -34px"
                              >640/ Month</v-list-item-subtitle
                            >
                          </v-list-item-content>
                          <v-tooltip class="d-flex align-end" top>
                            <template v-slot:activator="{ on, attrs }">
                              <v-btn icon v-bind="attrs" v-on="on">
                                <v-icon small color="grey lighten-1">
                                  mdi-information
                                </v-icon>
                              </v-btn>
                            </template>
                            <span class="tooltip-notification"
                              >Accounts. Learn More...</span
                            >
                          </v-tooltip>
                        </v-list-item>
                      </v-card>
                    </v-col>

                    <v-col cols="12" sm="6" md="6" lg="4">
                      <v-card
                        max-width="auto"
                        max-height="80"
                        outlined
                        hover
                        color="grey lighten-4"
                      >
                        <v-list-item three-line>
                          <v-list-item-avatar tile size="40">
                            <img
                              src="~assets/apps/expense.png"
                              alt="expense icon"
                            />
                          </v-list-item-avatar>

                          <v-list-item-content
                            style="margin-top: -20px"
                            class="text-capitalize"
                          >
                            Expense
                            <v-list-item-subtitle
                              style="
                                margin-top: -26px;
                                font-style: italic;
                                font-family: system-ui;
                                font-weight: 600;
                              "
                              >(Coming Soon...)</v-list-item-subtitle
                            >
                          </v-list-item-content>
                          <v-tooltip class="d-flex align-end" top>
                            <template v-slot:activator="{ on, attrs }">
                              <v-btn icon v-bind="attrs" v-on="on">
                                <v-icon small color="grey lighten-1">
                                  mdi-information
                                </v-icon>
                              </v-btn>
                            </template>
                            <span class="tooltip-notification"
                              >Expense. Learn More...</span
                            >
                          </v-tooltip>
                        </v-list-item>
                      </v-card>
                    </v-col>
                    <v-col cols="12" sm="6" md="6" lg="4">
                      <v-card
                        max-width="auto"
                        max-height="80"
                        outlined
                        hover
                        color="grey lighten-4"
                      >
                        <v-list-item three-line>
                          <v-list-item-avatar tile size="40">
                            <img
                              src="~assets/apps/fixed-assets.png"
                              alt="fixed assets icon"
                            />
                          </v-list-item-avatar>

                          <v-list-item-content
                            style="margin-top: -20px"
                            class="text-capitalize"
                          >
                            Fixed Assets
                            <v-list-item-subtitle
                              style="
                                margin-top: -26px;
                                font-style: italic;
                                font-family: system-ui;
                                font-weight: 600;
                              "
                              >(Coming Soon...)</v-list-item-subtitle
                            >
                          </v-list-item-content>
                          <v-tooltip class="d-flex align-end" top>
                            <template v-slot:activator="{ on, attrs }">
                              <v-btn icon v-bind="attrs" v-on="on">
                                <v-icon small color="grey lighten-1">
                                  mdi-information
                                </v-icon>
                              </v-btn>
                            </template>
                            <span class="tooltip-notification"
                              >Fixed Assets. Learn More...</span
                            >
                          </v-tooltip>
                        </v-list-item>
                      </v-card>
                    </v-col>

                    <v-col cols="12" sm="6" md="6" lg="4">
                      <v-card
                        max-width="auto"
                        max-height="80"
                        outlined
                        hover
                        color="grey lighten-4"
                      >
                        <v-list-item three-line>
                          <v-list-item-avatar tile size="40">
                            <img
                              src="~assets/apps/budget-planning.png"
                              alt="budget planning icon"
                            />
                          </v-list-item-avatar>

                          <v-list-item-content
                            style="margin-top: -20px"
                            class="text-capitalize"
                          >
                            Budget
                            <v-list-item-subtitle
                              style="
                                margin-top: -26px;
                                font-style: italic;
                                font-family: system-ui;
                                font-weight: 600;
                              "
                              >(Coming Soon...)</v-list-item-subtitle
                            >
                          </v-list-item-content>
                          <v-tooltip class="d-flex align-end" top>
                            <template v-slot:activator="{ on, attrs }">
                              <v-btn icon v-bind="attrs" v-on="on">
                                <v-icon small color="grey lighten-1">
                                  mdi-information
                                </v-icon>
                              </v-btn>
                            </template>
                            <span class="tooltip-notification"
                              >Budget Planning. Learn More...</span
                            >
                          </v-tooltip>
                        </v-list-item>
                      </v-card>
                    </v-col>
                  </v-row>
                </v-col>
                <!-- choose your apps ends here -->
                <!-- Second Col -->

                <!-- tab table begins here -->
                <v-col cols="12" sm="12" md="4" lg="4">
                  <v-app class="tab-table">
                    <v-card elevation="3">
                      <template>
                        <v-tabs centered light>
                          <label>
                            <v-tab style="color: #1976d2">
                              <input
                                type="radio"
                                class="form-radio text-indigo-600"
                                name="radio"
                                value="1"
                                checked
                              /><span style="margin-left: 4px">Annually</span>
                            </v-tab>
                          </label>
                          <label>
                            <v-tab style="color: #1976d2">
                              <input
                                style="color: #1976d2"
                                type="radio"
                                class="form-radio radio-bg"
                                name="radio"
                                value="1"
                              /><span style="margin-left: 4px"
                                >Monthly</span
                              ></v-tab
                            >
                          </label>
                          <v-tab-item>
                            <v-card flat>
                              <v-card-text
                                class="grey lighten-3"
                                style="color: #000"
                              >
                                {{ users }} Users<span class="float-right"
                                  ><span style="margin-right: 2px">₦</span
                                  >{{ appValue }}</span
                                >
                              </v-card-text>

                              <v-card-text
                                class="grey lighten-5"
                                style="color: #000"
                              >
                                User Discount<span class="float-right"
                                  >_ _ _</span
                                >
                              </v-card-text>

                              <v-card-text
                                class="grey lighten-3"
                                style="color: #000"
                              >
                                9 Apps<span class="float-right">{{
                                  eightyTimesUser() || '4800'
                                }}</span>
                              </v-card-text>

                              <v-card-text
                                class="grey lighten-5"
                                style="color: #000"
                              >
                                App Discount<span class="float-right"
                                  >_ _ _</span
                                >
                              </v-card-text>

                              <v-card-text
                                class="grey lighten-3"
                                style="color: #000"
                              >
                                Total / Month<span class="float-right"
                                  ><span style="margin-right: 2px">₦</span
                                  >4,632</span
                                >
                              </v-card-text>

                              <div class="grey lighten-5">
                                <v-card-text
                                  ><p
                                    class="font-weight-thin"
                                    style="color: #000"
                                  >
                                    Billed Annually<span class="float-right"
                                      ><span style="margin-right: 2px">₦</span
                                      >55,632</span
                                    >
                                  </p>
                                </v-card-text>
                                <div class="my-2 d-flex justify-center">
                                  <v-btn class="px-9" color="warning" dark>
                                    Try for free
                                  </v-btn>
                                </div>
                                <div class="my-2 d-flex justify-center">
                                  <v-btn class="px-14" color="success" dark>
                                    Buy Now
                                  </v-btn>
                                </div>
                              </div>
                            </v-card>
                          </v-tab-item>
                          <v-tab-item>
                            <v-card flat>
                              <v-card-text
                                class="grey lighten-3"
                                style="color: #000"
                              >
                                {{ users }} Users<span class="float-right"
                                  ><span style="margin-right: 2px">₦</span
                                  >{{ appValue }}</span
                                >
                              </v-card-text>

                              <v-card-text
                                class="grey lighten-5"
                                style="color: #000"
                              >
                                User Discount<span class="float-right"
                                  >_ _ _</span
                                >
                              </v-card-text>

                              <v-card-text
                                class="grey lighten-3"
                                style="color: #000"
                              >
                                9 Apps<span class="float-right">{{
                                  eightyTimesUser() || '4800'
                                }}</span>
                              </v-card-text>

                              <v-card-text
                                class="grey lighten-5"
                                style="color: #000"
                              >
                                App Discount<span class="float-right"
                                  >_ _ _</span
                                >
                              </v-card-text>

                              <v-card-text
                                class="grey lighten-3"
                                style="color: #000"
                              >
                                Total / Month<span class="float-right"
                                  ><span style="margin-right: 2px">₦</span
                                  >4,632</span
                                >
                              </v-card-text>

                              <div class="grey lighten-5">
                                <v-card-text
                                  ><p
                                    class="font-weight-thin"
                                    style="color: #000"
                                  >
                                    Billed Monthly<span class="float-right"
                                      ><span style="margin-right: 2px">₦</span
                                      >55,632</span
                                    >
                                  </p>
                                </v-card-text>
                                <div class="my-2 d-flex justify-center">
                                  <v-btn class="px-9" color="warning" dark>
                                    Try for free
                                  </v-btn>
                                </div>
                                <div class="my-2 d-flex justify-center">
                                  <v-btn class="px-14" color="success" dark>
                                    Buy Now
                                  </v-btn>
                                </div>
                              </div>
                            </v-card>
                          </v-tab-item>
                        </v-tabs>
                      </template>
                    </v-card>
                  </v-app>
                  <!-- tab table ends here -->
                </v-col>
              </v-row>
            </div>
          </div>
        </v-container>
      </v-app>
    </div>
  </no-ssr>
</template>

<script>
import AppHeader from './../components/header/AppHeader'
import PricingTabs from './../components/contents/PricingTabs'
export default {
  components: {
    AppHeader,
    PricingTabs,
  },
  data() {
    return {
      show: false,
      users: 1,
      appValue: '',
    }
  },
  methods: {
    // append(number) {
    //   this.appValue = `${this.appValue}${number}`
    // }
    eightyTimesUser() {
      this.appValue = this.users * 80
    },
  },

  head() {
    return {
      title: 'Cloudenly - Pricing',
      meta: [
        {
          hid: 'Cloudenly - Pricing',
          name: 'Cloudenly - Pricing',
          content:
            'Cloudenly - Flexible pricing options, from personal projects to enterprise applications, and everything in between',
        },
      ],
    }
  },
}
</script>
<style scoped>
/* Choose the number of users css */
.v-btn:not(.v-btn--round).v-size--default {
  height: 42px;
  min-width: 64px;
  padding: 0 16px;
}

.tooltip-notification {
  font-size: 12px;
  color: #fff;
}

.container-alignment {
  margin-left: 2px;
  margin-right: 2px;
}
* {
  font-family: GalanoGrotesque-Medium;
  /* color: #828282; */
}

h1 {
  line-height: 26px;
  font-size: 22px;
  font-weight: 500;
  margin-top: -50px;
}

.banner-h1 {
  margin-top: -50px;
  margin-bottom: 10px;
  padding: 10px 0;
  font-size: 36px;
  vertical-align: top;
  color: #fff;
}

.banner-p {
  font-size: 17px;
  text-align: center;
  margin: auto;
  color: #fff;
}

.banner {
  max-width: 100%;
  padding: 11rem 0 9rem 0;
  margin-top: 5rem;
  text-align: center;
  background-image: url('rectangle-banner.png');
  background-repeat: no-repeat;
  background-size: 100% 100%;
  color: white;
}

@media (max-width: 728px) {
  .banner-p {
    font-size: 16px;
  }

  .banner-h1 {
    font-size: 28px;
  }

  .banner {
    background-image: linear-gradient(
      268.51deg,
      #856fee 34.21%,
      #b894f6 73.36%
    );
  }
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

/* .v-application--wrap {
  min-height: 1px !important;
} */

/* @media (max-width: 480px) {
}
@media (max-width: 768px) {
}

@media (max-width: 1024px) {
}
@media (min-width: 1200px) {
} */
</style>
