<template>
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
              <v-list-item three-line>
                <v-list-item-avatar tile size="40">
                  <img src="~assets/apps/purchase.png" />
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
                  <img src="~assets/apps/sales.png" />
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
                  <span class="tooltip-notification">Sales. Learn More...</span>
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
                  <img src="~assets/apps/payments.png" />
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
                  <img src="~assets/apps/crm.png" />
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
                  <span class="tooltip-notification">CRM. Learn More...</span>
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
                  <img src="~assets/apps/expense.png" />
                </v-list-item-avatar>

                <v-list-item-content
                  style="margin-top: -20px"
                  class="text-capitalize"
                >
                  Expense
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
                  <img src="~assets/apps/accounts.png" />
                </v-list-item-avatar>

                <v-list-item-content
                  style="margin-top: -20px"
                  class="text-capitalize"
                >
                  Accounts
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
                  <img src="~assets/apps/inventory.png" />
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
                  <img src="~assets/apps/fixed-assets.png" />
                </v-list-item-avatar>

                <v-list-item-content
                  style="margin-top: -20px"
                  class="text-capitalize"
                >
                  Fixed Assets
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
                  <img src="~assets/apps/budget-planning.png" />
                </v-list-item-avatar>

                <v-list-item-content
                  style="margin-top: -20px"
                  class="text-capitalize"
                >
                  Budget Planning
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
                    >Budget Planning. Learn More...</span
                  >
                </v-tooltip>
              </v-list-item>
            </v-card>
          </v-col>
        </v-row>
      </v-col>
      <!-- Second Col -->
      <v-col cols="12" sm="12" md="4" lg="4">
        <TabTable />
      </v-col>
    </v-row>
  </div>
</template>

<script>
import TabTable from './TabTable'
export default {
  name: 'ChooseYourApps',
  components: {
    TabTable,
  },
  data() {
    return {
      show: false,
    }
  },
}
</script>

<style scoped>
.tooltip-notification {
  font-size: 12px;
  color: #fff;
}
* {
  font-family: GalanoGrotesque-Medium;
  /* color: #828282; */
}
</style>
