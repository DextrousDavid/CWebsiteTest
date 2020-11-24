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
                  <span class="ml-4">{{ cost }}</span>
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
                      <div :class="{ 'card-border': checkSelected('crm') }">
                        <v-card
                          max-width="auto"
                          max-height="80"
                          flat
                          link
                          color="grey lighten-4"
                          @click="addToAppsValue('crm')"
                        >
                          <!-- @click="append('640')" -->
                          <v-list-item three-line>
                            <v-list-item-avatar tile size="50">
                              <img src="~assets/apps/crm.svg" alt="crm icon" />
                            </v-list-item-avatar>

                            <v-list-item-content
                              style="margin-top: -10px"
                              class="text-capitalize black--text"
                            >
                              CRM
                              <v-list-item-subtitle
                                style="margin-top: -34px; font-size: 13px"
                                class="black--text"
                                >₦{{ crm }} / Month</v-list-item-subtitle
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
                                >CRM. Summary...</span
                              >
                            </v-tooltip>
                          </v-list-item>
                        </v-card>
                      </div>
                    </v-col>

                    <v-col cols="12" sm="6" md="6" lg="4">
                      <div
                        :class="{ 'card-border': checkSelected('purchase') }"
                      >
                        <v-card
                          max-width="auto"
                          max-height="80"
                          flat
                          color="grey lighten-4"
                          @click="addToAppsValue('purchase')"
                        >
                          <!-- @click="append('640')" -->
                          <!-- hover -->
                          <v-list-item three-line>
                            <v-list-item-avatar tile size="50">
                              <img
                                src="~assets/apps/purchase.svg"
                                alt="purchase icon"
                              />
                            </v-list-item-avatar>

                            <v-list-item-content
                              style="margin-top: -10px"
                              class="text--capitalize black--text"
                            >
                              Purchase
                              <v-list-item-subtitle
                                style="margin-top: -34px; font-size: 13px"
                                class="black--text"
                                >₦{{ purchase }} / Month</v-list-item-subtitle
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
                                >Purchase. Summary...</span
                              >
                            </v-tooltip>
                          </v-list-item>
                        </v-card>
                      </div>
                    </v-col>

                    <v-col cols="12" sm="6" md="6" lg="4">
                      <div :class="{ 'card-border': checkSelected('sales') }">
                        <v-card
                          max-width="auto"
                          max-height="80"
                          flat
                          link
                          color="grey lighten-4"
                          @click="addToAppsValue('sales')"
                        >
                          <v-list-item three-line>
                            <v-list-item-avatar tile size="50">
                              <img
                                src="~assets/apps/sales.svg"
                                alt="sales icon"
                              />
                            </v-list-item-avatar>

                            <v-list-item-content
                              style="margin-top: -10px"
                              class="text-capitalize black--text"
                              >Sales

                              <v-list-item-subtitle
                                style="margin-top: -34px; font-size: 13px"
                                class="black--text"
                                >₦{{ sales }} / Month</v-list-item-subtitle
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
                                >Sales. Summary...</span
                              >
                            </v-tooltip>
                          </v-list-item>
                        </v-card>
                      </div>
                    </v-col>

                    <v-col cols="12" sm="6" md="6" lg="4">
                      <div
                        :class="{ 'card-border': checkSelected('inventory') }"
                      >
                        <v-card
                          max-width="auto"
                          max-height="80"
                          flat
                          link
                          color="grey lighten-4"
                          @click="addToAppsValue('inventory')"
                        >
                          <v-list-item three-line>
                            <v-list-item-avatar tile size="50">
                              <img
                                src="~assets/apps/inventory.svg"
                                alt="inventory icon"
                              />
                            </v-list-item-avatar>

                            <v-list-item-content
                              style="margin-top: -10px"
                              class="text-capitalize black--text"
                            >
                              Inventory
                              <v-list-item-subtitle
                                style="margin-top: -34px; font-size: 13px"
                                class="black--text"
                                >₦{{ inventory }} / Month</v-list-item-subtitle
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
                                >Inventory. Summary...</span
                              >
                            </v-tooltip>
                          </v-list-item>
                        </v-card>
                      </div>
                    </v-col>
                    <v-col cols="12" sm="6" md="6" lg="4">
                      <v-card
                        max-width="auto"
                        max-height="80"
                        flat
                        link
                        color="grey lighten-4"
                      >
                        <v-list-item three-line>
                          <v-list-item-avatar tile size="50">
                            <img
                              src="~assets/apps/payments.svg"
                              alt="payments icon"
                            />
                          </v-list-item-avatar>

                          <v-list-item-content
                            style="margin-top: -10px"
                            class="text-capitalize black--text"
                          >
                            Payments
                            <v-list-item-subtitle
                              style="margin-top: -34px"
                              class="black--text"
                              >Free</v-list-item-subtitle
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
                              >Payments. Summary...</span
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
                      >
                        <v-list-item three-line>
                          <v-list-item-avatar tile size="50">
                            <img
                              src="~assets/apps/accounting.svg"
                              alt="accounts icon"
                            />
                          </v-list-item-avatar>

                          <v-list-item-content
                            style="margin-top: -10px"
                            class="text-capitalize black--text"
                          >
                            Accounting
                            <v-list-item-subtitle
                              style="margin-top: -34px"
                              class="black--text"
                              >Free</v-list-item-subtitle
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
                              >Accounting. Summary...</span
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
                      >
                        <v-list-item three-line>
                          <v-list-item-avatar tile size="50">
                            <img
                              src="~assets/apps/expense.svg"
                              alt="expense icon"
                            />
                          </v-list-item-avatar>

                          <v-list-item-content
                            style="margin-top: -10px"
                            class="text-capitalize black--text"
                          >
                            Expense
                            <v-list-item-subtitle
                              style="
                                margin-top: -31px;
                                font-style: italic;
                                font-family: system-ui;
                                font-weight: 600;
                                font-size: 11px;
                              "
                              class="black--text"
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
                              >Expense. Summary...</span
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
                      >
                        <v-list-item three-line>
                          <v-list-item-avatar tile size="50">
                            <img
                              src="~assets/apps/fixed-assets.svg"
                              alt="fixed assets icon"
                            />
                          </v-list-item-avatar>

                          <v-list-item-content
                            style="margin-top: -10px"
                            class="text-capitalize black--text"
                          >
                            Fixed Assets
                            <v-list-item-subtitle
                              style="
                                margin-top: -31px;
                                font-style: italic;
                                font-family: system-ui;
                                font-weight: 600;
                                font-size: 11px;
                              "
                              class="black--text"
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
                              >Fixed Assets. Summary...</span
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
                      >
                        <v-list-item three-line>
                          <v-list-item-avatar tile size="50">
                            <img
                              src="~assets/apps/budget.svg"
                              alt="budget planning icon"
                            />
                          </v-list-item-avatar>

                          <v-list-item-content
                            style="margin-top: -10px"
                            class="text-capitalize black--text"
                          >
                            Budget
                            <v-list-item-subtitle
                              style="
                                margin-top: -31px;
                                font-style: italic;
                                font-family: system-ui;
                                font-weight: 600;
                                font-size: 11px;
                              "
                              class="black--text"
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
                              >Budget Planning. Summary...</span
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
                            <v-tab
                              style="color: #1976d2"
                              @click="userPerAnnual"
                            >
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
                            <v-tab style="color: #1976d2" @click="userPerMonth">
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
                                {{ users }}
                                <span>{{ userToUsersText() }}</span
                                ><span class="float-right"
                                  >₦{{ annualTimesUser }}</span
                                >
                              </v-card-text>

                              <v-card-text
                                class="grey lighten-5"
                                style="color: #000"
                              >
                                User Discount<span
                                  style="color: #ff0000"
                                  class="float-right"
                                  >-₦{{
                                    annualUserDiscountOnInitialPurchase
                                  }}</span
                                >
                              </v-card-text>

                              <v-card-text
                                class="grey lighten-3"
                                style="color: #000"
                              >
                                {{ products.length }} {{ appToAppsText()
                                }}<span class="float-right"
                                  >₦{{ appsValueAnnually }}</span
                                >
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
                                  ><span class="float-right"
                                    >₦{{ totalPerMonthAnnualForAnnual }}</span
                                  ></span
                                >
                              </v-card-text>

                              <div class="grey lighten-5">
                                <v-card-text
                                  ><p
                                    class="font-weight-thin"
                                    style="color: #000"
                                  >
                                    Billed Annually<span class="float-right"
                                      ><span class="float-right"
                                        >₦{{ billedAnnualTimesUser }}</span
                                      ></span
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
                                {{ users }} <span>{{ userToUsersText() }}</span
                                ><span class="float-right"
                                  >₦{{ monthlyTimesUser }}</span
                                >
                              </v-card-text>

                              <v-card-text
                                class="grey lighten-5"
                                style="color: #000"
                              >
                                User Discount<span
                                  style="color: #ff0000"
                                  class="float-right"
                                  >-₦{{
                                    monthlyUserDiscountOnInitialPurchase
                                  }}</span
                                >
                              </v-card-text>

                              <v-card-text
                                class="grey lighten-3"
                                style="color: #000"
                              >
                                {{ products.length }} {{ appToAppsText()
                                }}<span class="float-right"
                                  >₦{{ appsValueMonthly }}</span
                                >
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
                                  ><span class="float-right"
                                    >₦{{ totalPerMonthAnnualForMonthly }}</span
                                  ></span
                                >
                              </v-card-text>

                              <div class="grey lighten-5">
                                <v-card-text
                                  ><p
                                    class="font-weight-thin"
                                    style="color: #000"
                                  >
                                    Billed Monthly<span class="float-right"
                                      >₦{{ billedMonthlyTimesUser }}</span
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
      prices: {
        crm: 3499,
        purchase: 2699,
        sales: 2699,
        inventory: 5499,
      },
      products: [],
      show: false,
      users: 1,
      apps: 0,
      appsValueMonthly: 0,
      appsValueAnnually: 0,
      // cost here being synanimous with choose your apps
      cost: '₦2799 / User / Month',
      crm: 2799,
      purchase: 2159,
      sales: 2159,
      inventory: 4399,
      isActive: true,
      // appValue uses eightyTimesUser method value
    }
  },
  computed: {
    // ANNUAL SUBSCRIPTION CALCULATION STARTS HERE *******
    // multiplies 2799 with the total number of users
    annualTimesUser() {
      return this.users * 2799
    },

    // multiplies 2799 and total number number of users, then divides by 2
    annualUserDiscountOnInitialPurchase() {
      return Math.round((this.users * 2799) / 2)
    },

    // Total / Month multiplies annualTimesUser with annualUserDiscountOnInitialPurchase functions!
    totalPerMonthAnnualForAnnual() {
      return this.annualTimesUser - this.annualUserDiscountOnInitialPurchase
    },
    // multiplies totalPerMonthAnual  by 12 (annual)
    billedAnnualTimesUser() {
      return this.totalPerMonthAnnualForAnnual * 12
    },

    // MONTHLY SUBSCRIPTION CALCULATION STARTS HERE *******
    // multiplies 3499 with the total number of users
    monthlyTimesUser() {
      return this.users * 3499
    },
    // multiplies 3499 and total number number of users, then divides by 2
    monthlyUserDiscountOnInitialPurchase() {
      return Math.round((this.users * 3499) / 2)
    },

    // Total / Month multiplies annualTimesUser with annualUserDiscountOnInitialPurchase functions!
    totalPerMonthAnnualForMonthly() {
      return this.monthlyTimesUser - this.monthlyUserDiscountOnInitialPurchase
    },
    // multiplies totalPerMonthAnual  by 12 (annual)
    billedMonthlyTimesUser() {
      return this.totalPerMonthAnnualForMonthly
    },
  },
  methods: {
    checkSelected(value) {
      return this.products.includes(value)
    },
    addToAppsValue(value) {
      let products = this.products

      if (products.includes(value)) {
        products = products.filter((el) => el !== value)
        this.removePrice(value)
      } else {
        products.push(value)
        this.calculateApps(value)
      }
      this.products = products
    },
    calculateApps(value) {
      let appsValueMonthly = this.appsValueMonthly
      const appsValueAnnually = this.appsValueAnnually
      let valuePrice = 0

      const percentDisount = 0.2
      let discount = 0

      switch (value) {
        case 'crm':
          appsValueMonthly = appsValueMonthly + this.prices.crm
          this.appsValueMonthly = appsValueMonthly

          valuePrice = this.prices.crm
          discount = Math.round(valuePrice * percentDisount)
          valuePrice = valuePrice - discount
          this.appsValueAnnually = appsValueAnnually + valuePrice
          break
        case 'purchase':
          appsValueMonthly = appsValueMonthly + this.prices.purchase
          this.appsValueMonthly = appsValueMonthly

          valuePrice = this.prices.purchase
          discount = Math.round(valuePrice * percentDisount)
          valuePrice = valuePrice - discount
          this.appsValueAnnually = appsValueAnnually + valuePrice
          break
        case 'sales':
          appsValueMonthly = appsValueMonthly + this.prices.sales
          this.appsValueMonthly = appsValueMonthly

          valuePrice = this.prices.sales
          discount = Math.round(valuePrice * percentDisount)
          valuePrice = valuePrice - discount
          this.appsValueAnnually = appsValueAnnually + valuePrice
          break
        case 'inventory':
          appsValueMonthly = appsValueMonthly + this.prices.inventory
          this.appsValueMonthly = appsValueMonthly

          valuePrice = this.prices.inventory
          discount = Math.round(valuePrice * percentDisount)
          valuePrice = valuePrice - discount
          this.appsValueAnnually = appsValueAnnually + valuePrice
          break

        default:
          break
      }
    },
    removePrice(value) {
      let appsValueMonthly = this.appsValueMonthly
      let appsValueAnnually = this.appsValueAnnually
      let annualPrice = 0

      const percentDisount = 0.2
      let discount = 0

      switch (value) {
        case 'crm':
          appsValueMonthly = appsValueMonthly - this.prices.crm
          this.appsValueMonthly = appsValueMonthly

          annualPrice = this.prices.crm

          discount = Math.round(annualPrice * percentDisount)

          annualPrice = annualPrice - discount
          appsValueAnnually = appsValueAnnually - annualPrice
          this.appsValueAnnually = appsValueAnnually
          break
        case 'purchase':
          appsValueMonthly = appsValueMonthly - this.prices.purchase
          this.appsValueMonthly = appsValueMonthly

          annualPrice = this.prices.purchase

          discount = Math.round(annualPrice * percentDisount)

          annualPrice = annualPrice - discount
          appsValueAnnually = appsValueAnnually - annualPrice
          this.appsValueAnnually = appsValueAnnually
          break
        case 'sales':
          appsValueMonthly = appsValueMonthly - this.prices.sales
          this.appsValueMonthly = appsValueMonthly

          annualPrice = this.prices.sales

          discount = Math.round(annualPrice * percentDisount)

          annualPrice = annualPrice - discount
          appsValueAnnually = appsValueAnnually - annualPrice
          this.appsValueAnnually = appsValueAnnually
          break
        case 'inventory':
          appsValueMonthly = appsValueMonthly - this.prices.inventory
          this.appsValueMonthly = appsValueMonthly

          annualPrice = this.prices.inventory

          discount = Math.round(annualPrice * percentDisount)

          annualPrice = annualPrice - discount
          appsValueAnnually = appsValueAnnually - annualPrice
          this.appsValueAnnually = appsValueAnnually
          break
        default:
          break
      }
    },
    // changes user to users text
    userToUsersText() {
      if (this.users > 1) {
        return 'Users'
      } else {
        return 'User'
      }
    },
    appToAppsText() {
      if (this.products.length > 1) {
        return 'Apps'
      } else {
        return 'App'
      }
    },

    // 2799 user / month
    userPerAnnual() {
      this.cost = '₦2799 / User / Month'
      this.crm = 2799
      this.purchase = 2159
      this.sales = 2159
      this.inventory = 4399
    },
    userPerMonth() {
      this.cost = '₦3499 / User / Month'
      this.crm = 3499
      this.purchase = 2699
      this.sales = 2699
      this.inventory = 5499
    },
  },
  // methods: {
  //   eightyTimesUser() {
  //     this.appValue = this.users * 80
  //   },
  // },

  // data: () => ({
  //   currentItem: 'tab-Web',
  //   items: ['Web', 'Shopping', 'Videos', 'Images'],
  //   more: ['News', 'Maps', 'Books', 'Flights', 'Apps'],
  // }),

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
.card-border {
  border: 2px solid;
  border-image-source: linear-gradient(
    45deg,
    rgb(84 219 241),
    rgb(250 159 66 / 85%)
  );
  border-image-slice: 1;
}
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
