<template>
  <no-ssr>
    <div>
      <AccordionHeader />
      <section class="banner mb-8">
        <div class="content-center mr-3 ml-3">
          <h1 class="banner-h1">How can we help you?</h1>
          <div style="max-width: 550px; margin: auto">
            <p class="banner-p font-normal">
              Find help and learning resources below
            </p>
          </div>
        </div>
      </section>
      <div class="mt-12 mb-8 flex items-center text-center justify-center">
        <div class="rounded-lg">
          <img
            class="mr-3 inline-block"
            src="~assets/userguideIcons/Optima1.png"
            alt="Optima logo"
          />
          <h1 class="font-bold inline-block" style="color: #333">Optima</h1>
          <!-- The one below Doesnt look to Good -->
          <!-- <h2 class="-ml-24 my-3">User Guide</h2> -->
          <h3 class="ml-8 -mt-2 font-semibold">User Guide</h3>
        </div>
      </div>

      <!-- main content -->
      <main>
        <no-ssr>
          <Accordion :user-guides="userGuides" />
        </no-ssr>
      </main>
    </div>
  </no-ssr>
</template>

<script>
// import Banner from '../../../components/contents/Banner'
import AccordionHeader from '../../../components/contents/AccordionHeader'
import Accordion from '../../../components/contents/Accordion'

export default {
  components: {
    AccordionHeader,
    // Banner,
    Accordion,
  },
  data() {
    return {
      userGuides: [
        {
          id: 1,
          heading: 'Get Started With Optima',
          content1: 'How do i log in on the app?',
          content2: 'Tips and Tricks of Optima',
          content3: 'Get started with Optima',
        },
        {
          id: 2,
          content1: 'Customer Relationship Management (CRM)',
          url1:
            'https://resources.cloudenly.com/knowledge-base/customer-relationship-management-crm/',
          heading: 'Customer Relationship Management (CRM)',
          content2: 'Customer Registration',
          url2:
            'https://resources.cloudenly.com/knowledge-base/customer-registration/',
          content3: 'Customer Engagement',
          url3:
            'https://resources.cloudenly.com/knowledge-base/customer-engagement/',
          content4: 'Pipeline Management',
          url4:
            'https://resources.cloudenly.com/knowledge-base/pipeline-management/',
          content5: 'Promotions',
          url5: 'https://resources.cloudenly.com/knowledge-base/promotion/',
          content6: 'Meeting',
          url6: 'https://resources.cloudenly.com/knowledge-base/meeting/',
        },
        {
          id: 3,
          heading: 'Purchase',
          content1: 'Purchase',
          url1: 'https://resources.cloudenly.com/knowledge-base/purchase/',
          content2: 'Supplier',
          url2: 'https://resources.cloudenly.com/knowledge-base/supplier/',
          content3: 'Catalogue',
          url3:
            'https://resources.cloudenly.com/knowledge-base/purchase-catalogue/',
          content4: 'Purchase Requisition',
          url4:
            'https://resources.cloudenly.com/knowledge-base/purchase-requisition-pr/',
          content5: 'Request for Quote (RFQ)',
          url5:
            'https://resources.cloudenly.com/knowledge-base/request-for-quote-rfq/',
          content6: 'Quote',
          url6:
            'https://resources.cloudenly.com/knowledge-base/purchase-quote/',
          content7: 'Purchase Order (PO)',
          url7:
            'https://resources.cloudenly.com/knowledge-base/purchase-order-po/',
          content8: 'Invoice',
          url8: 'https://resources.cloudenly.com/knowledge-base/invoice-2/',
          content9: 'Debit Note',
          url9: 'https://resources.cloudenly.com/knowledge-base/debit-note/',
        },
        {
          id: 4,
          heading: 'Sales',
          content1: 'Sales',
          url1: 'https://resources.cloudenly.com/knowledge-base/sales/',
          content2: 'Catalogue',
          url2:
            'https://resources.cloudenly.com/knowledge-base/sales-catalogue/',
          content3: 'Pricebook',
          url3: 'https://resources.cloudenly.com/knowledge-base/price-book/',
          content4: 'Request for Quote (RFQ)',
          url4:
            'https://resources.cloudenly.com/knowledge-base/sales-request-for-quote/',
          content5: 'Quote',
          url5: 'https://resources.cloudenly.com/knowledge-base/sales-quote/',
          content6: 'Purchase Order (PO)',
          url6:
            'https://resources.cloudenly.com/knowledge-base/sales-purchase-order/',
          content7: 'Invoice',
          url7: 'https://resources.cloudenly.com/knowledge-base/invoice/',
          content8: 'Waybill',
          url8:
            'https://resources.cloudenly.com/knowledge-base/waybill-sales-order/',
          content9: 'Credit Note',
          url9: 'https://resources.cloudenly.com/knowledge-base/credit-notes/',
        },
        {
          id: 5,
          heading: 'Inventory',
          content1: 'Inventory',
          url1: 'https://resources.cloudenly.com/knowledge-base/inventory/',
          content2: 'Outlets and Inventory Classes',
          url2:
            'https://resources.cloudenly.com/knowledge-base/outlet-and-inventory-class/',
          content3: 'Stock Balance',
          url3:
            'https://resources.cloudenly.com/knowledge-base/inventory-operations/',
          content4: 'Waybill',
          url4:
            'https://resources.cloudenly.com/knowledge-base/inventory-waybill/',
          content5: 'Goods Received Note',
          url5:
            'https://resources.cloudenly.com/knowledge-base/inventory-goods-received-note-grn/',
          content6: 'Material Request',
          url6:
            'https://resources.cloudenly.com/knowledge-base/material-request/',
          content7: 'Material Return',
          url7: '',
        },
        {
          id: 6,
          heading: 'Production',
          content1: 'Production',
          url1: '',
        },
        {
          id: 7,
          heading: 'Finance',
          content1: 'Finance',
          url1: '',
        },
        {
          id: 8,
          heading: 'Payment',
          content1: 'Payment',
          url1: '',
        },
        {
          id: 9,
          heading: 'Accounts',
          content1: 'Accounts',
          url1: '',
        },
        {
          id: 10,
          heading: 'Approval Center',
          content1: 'Approval Center',
          url1: '',
        },
        {
          id: 11,
          heading: 'Settings',
          content1: 'Settings',
          url1: '',
        },
      ],
    }
  },
  head() {
    return {
      title: 'User Guide - Optima',
      meta: [
        {
          hid: 'User Guide - Optima',
          name: 'User Guide - Optima',
          content: 'Tips and Tricks of Optima, Get started with Optima.',
        },
      ],
    }
  },
}
</script>

<style scoped>
* {
  font-family: GalanoGrotesque-Medium;
  color: #828282;
}

h1 {
  font-size: 40px;
  margin-bottom: -20px;
  margin-left: -8px;
}

h2 {
  font-size: 20px;
}

img {
  margin-top: -28px;
  height: 80px;
}
/* .resource-card {
  padding: 40px 6px 15px 6px;
  border-radius: 6px;
  border: 2px solid #f4f4f4;
  margin-bottom: 40px;
}

h1 {
  line-height: 26px;
  font-size: 22px;
  font-weight: 500;
  margin-top: -50px;
}

h5 {
  margin-top: 20px;
  font-size: 14px;
  margin-bottom: 20px;
}

.userguideicons {
  width: 50%;
  margin: auto;
} */
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
  background-image: url('rectangle3.jpg');
  background-repeat: no-repeat;
  background-size: 100% 100%;
  color: white;
}

@media (max-width: 728px) {
  .banner-p {
    font-size: 15px;
  }

  .banner-h1 {
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
