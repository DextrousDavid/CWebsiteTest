<template>
  <div>
    <div class="our-product">
      <div class="cloudenly-headline" style="text-align: center">
        Our Product Pack
      </div>
      <div class="w-full sm:flex justify-center tabs-container">
        <div class="tabs-control">
          <v-tabs v-model="currentTab" background-color="transparent" grow>
            <v-tab>Optima</v-tab>
            <v-tab>HumanaR</v-tab>
            <v-tab>Dome</v-tab>
          </v-tabs>
        </div>
        <v-tabs-items v-model="currentTab">
          <v-tab-item>
            <Product v-bind:features="optima_content" />
          </v-tab-item>
          <v-tab-item>
            <Product v-bind:features="optima_content"/>
          </v-tab-item>
          <v-tab-item>
            <Product v-bind:features="optima_content"/>
          </v-tab-item>
        </v-tabs-items>
      </div>
    </div>
  </div>
</template>
<script>
import Product from './Product'
export default {
  components: {
    Product,
  },
  data() {
    return {
      currentTab: null,
      optima_content: [
        {
          header: 'CRM',
          content: `Contact Registration, Customer Engagement, Pipeline
                    Management, Loyalty & Promo`,
        },
        {
          header: 'Supply Chain',
          content: `Supplier Management, Product Catalog, Price Book, Quotes and
                    Invoice Management, Multi-Outlet/Multi- Inventory
                    Operations, Inventory Valuation, Material Management.`,
        },
        {
          header: 'Account Management',
          content: `Account Receivables, Account Payables, Revenue, Expense,
                    Profits & Loss, Assets & Liabilities.`,
        },
        {
          header: '	Analytics & Business Intelligence',
        },
        {
          header: 'Commerce Cloud',
          content: `PoS, Marketplace integrations`,
        },
        {
          header: 'Production Management',
          content: `Material Requirement Planning, Material Assembly, Job
                    Orders, Material Request, Production Management`,
        },
        {
          header: 'Finance Management (Coming Soon)',
          content: `Expense Management, Budget Planning & Management`,
        },
        {
          header: 'Payment',
          content: `Payment & collection`,
        },
      ],
    }
  },
}
</script>
<style scoped>
.our-product {
  background: #ffffff;
  padding: 100px 68px;
}

.tabs-container {
  margin-top: 20px;
  flex-direction: column;
  align-items: center;
}
.tabs-control {
}
</style>
<style>
.tabs-control .v-tab {
  font-size: 16px;
  line-height: 19px;
  font-family: GalanoGrotesque-SemiBold;
}
</style>
