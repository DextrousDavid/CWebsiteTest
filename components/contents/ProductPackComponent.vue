<template>
  <div>
    <div class="our-product">
      <div class="cloudenly-headline" style="text-align: center">
        Our Product Pack
      </div>
      <div class="w-full sm:flex justify-center tabs-container">
        <div
          class="tabs-control"
          :class="
            currentTab == 1
              ? 'domeActive'
              : currentTab == 2
              ? 'humanaActive'
              : null
          "
        >
          <v-tabs v-model="currentTab" background-color="transparent" grow>
            <!-- <v-tab>Ally</v-tab> -->
            <v-tab>Dome</v-tab>
            <v-tab>HumanaR</v-tab>
            <v-tab>Optima</v-tab>
            <v-tab>Quantum</v-tab>
          </v-tabs>
        </div>

        <v-tabs-items v-model="currentTab">
          <!-- <v-tab-item>
            <div></div>
          </v-tab-item> -->
          <v-tab-item>
            <Product :features="dome_content" />
          </v-tab-item>
          <v-tab-item>
            <Product :features="humana_content" />
          </v-tab-item>
          <v-tab-item>
            <Product :features="optima_content" />
          </v-tab-item>
          <v-tab-item>
            <Product :features="quantum_content" />
          </v-tab-item>
        </v-tabs-items>
      </div>
    </div>
  </div>
</template>
<script>
// import { VTabs, VTab, VTabItem, VTabsItems } from 'vuetify/lib'
import Product from './Product'
export default {
  components: {
    Product,
    // VTabItem,
    // VTabsItems,
    // VTabs,
    // VTab,
  },
  data() {
    return {
      currentTab: 2,
      optima_content: [
        {
          header: 'CRM',
          content: `Contact Registration, Customer Engagement, Pipeline 
Management, Loyalty & Promos`,
        },
        {
          header: 'Purchase',
          content: `Supplier Management, Product Catalog, Purchase
 Requisition, Request for Quote, Quotes, Purchase 
Orders, Invoice, Debit Notes`,
        },
        {
          header: 'Sales',
          content: `Supplier Management, Product Catalog, Price Book,
 Quotes, Purchase Orders, Invoice, Credit Notes.`,
        },
        {
          header: '	Inventory',
          content: `Multi-Outlet/Multi-Inventory Operations,
 Inventory Valuation, Stock Management.`,
        },
        {
          header: 'Payment',
          content: `Payment & collection`,
        },
        {
          header: 'Commerce Cloud',
          content: `PoS, Marketplace integrations`,
        },
        {
          header: 'Production Management (Coming Soon)',
          content: `Material Requirement Planning, Material Assembly, Job
                    Orders, Material Request, Production Management`,
        },
        {
          header: '	Accounting',
          content: `Chart of Accounts, Cost Centers, Expense Codes, 
Account Receivables, Account Payables, Revenue,
Expense, Profits & Loss, Assets & Liabilities.`,
        },
        {
          header: `Budget, Asset and Expense Management
(Coming Soon)`,
          content: `Expense Management, BudgetPlanning & Management`,
        },
        {
          header: `Analytics & Business Intelligence`,
        },
      ],
      humana_content: [
        {
          header: 'Organisation Design',
          content: `Functions, Job Levels, Designations, People`,
        },
        {
          header: 'Employees',
          content: ` Employee Directory, Groups, Employee Engagement,
 Delegation Management.`,
        },
        {
          header: 'Benfit Adminstration',
          content: `Leave of Absence, Advances & Loans, Overtime`,
        },
        {
          header: 'HR Documentation',
          content: `Organisation Documents and Employee Documents.`,
        },
        {},
        {
          header: 'Payroll',
          content: `Pay Runs, PAYE, Pension.`,
        },
        {
          header: 'Performance Management (Coming Soon)',
          content: `Performance Goals, Key Performance Agreements,
Performance Reviews & Moderations, Performance
Improvement Plans, 360 Degrees Feedback`,
        },
        {
          header: 'Finance  (Coming Soon)',
          content: ` Expense Management, Advances & Loans, 
 Asset Management)`,
        },
        {
          header: 'HRBP & Advisory Service (Coming Soon)',
          // content: `Payment & collection`,
        },
        {
          header: '	Analytics & Business Intelligence',
          // content: `Payment & collection`,
        },
      ],
      dome_content: [
        {
          header: 'Content Management',
          content: `Folders & Files`,
        },
        {
          header: 'Collaboration',
          content: `Share, Edit, Comment..`,
        },
        {
          header: 'User Management',
          content: `Groups, Users, Capacity Mgt., Activity Logs`,
        },
        {
          header: '',
        },
        {
          header: '',
        },
        {
          header: 'Security',
          content: `Password Policy Enforcement, Two Factor
Authentication, Data Loss Prevention, Security Logs`,
        },
        {
          header: 'Advanced Control (Coming Soon)',
          content: `Dynamic Version Management, Usage
Analytics, etc.`,
        },
        {
          header: '',
        },
        {
          header: 'Analytics & Business Intelligence',
        },
      ],
      quantum_content: [
        {
          header: 'Account Profile',
          content: `Organisation, Root Admin`,
        },
        {
          header: 'Organsation',
          content: `Functions, Job Levels, Designations,	People.`,
        },
        {
          header: 'Payments & Collection',
          content: `Currency, Payments, Collections`,
        },
        {
          header: 'Location & Tax',
          content: ` Outlets & Offices, Tax ,Remittance.`,
        },
        {
          header: 'Notification & Messaging',
          content: `Subscription Management`,
        },
        {
          header: 'Security Policy',
          content: `Password Protection, Security Question, 
Two Factor Authentication (2FA), IP Fencing`,
        },
        {
          header: 'Identify & Access Management',
          content: `User Roles, Privilege settings.`,
        },
        {
          header: 'Users & Groups',
          content: `Users, Groups.`,
        },
        {
          header: `Approval Flow`,
          content: ` Automatic Set up, Manual Set up.`,
        },
        {
          header: `Activity & Audit Log`,
          content: `Active Users, Access Reports, Failed Login Reports.`,
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
@media (max-width: 768px) {
  .our-product {
    padding: 0px 0px;
  }
}
</style>
<style>
.tabs-control .v-tab {
  font-size: 16px;
  line-height: 19px;
  font-family: GalanoGrotesque-SemiBold;
}

.tabs-control .v-tabs-slider-wrapper .v-tabs-slider {
  background-color: unset;
}
.tabs-control .v-tab.v-tab--active {
  font-family: GalanoGrotesque-SemiBold;
  font-size: 16px;
  line-height: 19px;
  color: #f1f5fb;
  background: #4781dc;
  border-radius: 3px;
}
.domeActive .v-tab.v-tab--active {
  background: #05613a !important;
}
.humanaActive .v-tab.v-tab--active {
  background: #5e227f !important;
}
.qunatumActive .v-tab.v-tab--active {
  background: #5e227f !important;
}
</style>
