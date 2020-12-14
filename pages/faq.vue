<template>
  <no-ssr>
    <div>
      <AppHeader />
      <!-- Remove shadow outline to remove outlines that appears when you click on a button or input (Focus focus:shadow-outline?) === focus:outline-none -->
      <!-- Banner Starts here -->
      <section class="banner mb-8">
        <div class="content-center mr-3 ml-3">
          <h1 class="banner-h1">Frequently Asked Questions</h1>
          <div style="max-width: 550px; margin: auto">
            <!-- <p class="banner-p font-normal">
            Our technical teams are currently facing a significant increase in
            the number of support requests. You may experience a delayed
            response time as we work to address this.
          </p> -->
          </div>
        </div>
      </section>
      <!-- Banner Ends here -->
      <div class="mt-12 mb-8 flex items-center text-center justify-center">
        <div class="rounded-lg">
          <img
            style="width: 13rem"
            src="/img/cloudenly-logo.svg"
            alt="Cloudenlylogo"
          />

          <!-- The one below Doesnt look to Good -->
          <!-- <h2 class="-ml-24 my-3">User Guide</h2> -->
          <!-- <h3 class="ml-8 -mt-2 font-semibold">User Guide</h3> -->
        </div>
      </div>
      <main>
        <v-app>
          <v-container>
            <v-row>
              <v-col cols="12" sm="6" md="4">
                <h4 class="h4 flex font-bold">About Cloudenly and Scelloo</h4>
              </v-col>
              <v-col cols="12" sm="6" md="8">
                <FaqAccordion :faqs="faqs1" />
              </v-col>
            </v-row>

            <v-row>
              <v-col cols="12" sm="6" md="4">
                <div>
                  <h4 class="h4 flex font-bold">Getting Started</h4>
                </div>
              </v-col>
              <v-col cols="12" sm="6" md="8">
                <FaqAccordion :faqs="faqs2" />
              </v-col>
            </v-row>

            <v-row>
              <v-col cols="12" sm="6" md="4">
                <div>
                  <p class="h4 flex font-bold">Payment</p>
                </div>
              </v-col>
              <v-col cols="12" sm="6" md="8">
                <FaqAccordion :faqs="faqs3" />
              </v-col>
            </v-row>

            <v-row>
              <v-col cols="12" sm="6" md="4">
                <div>
                  <p class="h4 flex font-bold">About Data and Security</p>
                </div>
              </v-col>
              <v-col cols="12" sm="6" md="8">
                <FaqAccordion :faqs="faqs4" />
              </v-col>
            </v-row>

            <v-row>
              <v-col cols="12" sm="6" md="4">
                <div>
                  <p class="h4 flex font-bold">Product Features</p>
                </div>
              </v-col>
              <v-col cols="12" sm="6" md="8">
                <FaqAccordion :faqs="faqs5" />
              </v-col>
            </v-row>

            <v-row>
              <v-col cols="12" sm="6" md="4">
                <div>
                  <p class="h4 flex font-bold">Support</p>
                </div>
              </v-col>
              <v-col cols="12" sm="6" md="8">
                <FaqAccordion :faqs="faqs6" />
              </v-col>
            </v-row>
          </v-container>
        </v-app>
      </main>
    </div>
  </no-ssr>
</template>

<script>
import AppHeader from './../components/header/AppHeader'
import FaqAccordion from './../components/contents/FaqAccordion'
export default {
  components: {
    AppHeader,
    FaqAccordion,
  },
  data() {
    return {
      faqs1: [
        {
          id: 1,
          heading: 'What is the relationship between Scelloo and Cloudenly?',
          content1:
            'Cloudenly is a product suite of Scelloo a technology company that harnesses the value of technology to provide solutions to help entrepreneurs and organizations thrive.',
        },
        {
          id: 2,
          heading: "What is Cloudenly's product suite?",
          content1:
            'Cloudenly is an Enterprise Resource Planning (ERP) application with the following products:',
          content2:
            '• <b>Optima</b> - An integrated supply chain and accounting solution',

          content3:
            '• <b>HumanaR</b> - The integrated HR operations and people experience management platform ',

          content4:
            '• <b>Dome</b> - Secure file sharing and storage for teams with access control. – <em>Coming soon</em>',
        },
        {
          id: 3,
          heading: 'How are Cloudenly products offered?',
          content1:
            'Cloudenly products are offered to customers primarily as “Software as a Service” (SaaS) applications and are preconfigured to fit most organization’s needs. Organizations have the flexibility to customize these products to fit their specific needs. Usage is generally subscription-based, with the option to pay monthly or annually. Cloudenly products, being cloud-based means that users do not have to worry about it being expensive and most often, challenging upgrades.',
        },
      ],
      faqs2: [
        {
          id: 1,
          heading:
            'Do I need a lot of money to get started on the Cloudenly software?',
          content1:
            'No, you don’t. Our software is available for a monthly token as a Software-as-a-Service (SaaS), and you can access the service from anywhere through a browser.',
          content2: 'Sign up for free or Contact us for assistance',
        },
        {
          id: 2,
          heading:
            'I am not sure which product works for my business in the Cloudenly suite',
          content1:
            '<b>Micro Enterprises</b>: Are you a solo enterprise with basic business processes and bootstrapping your way to success? If this sounds like you then Lite is for you.',
          content2: 'Sign up for free or Contact us for assistance.',
          content3:
            '<b>Small, Medium & Large Enterprise</b>: Do you have a growing team and looking at ways to scale your business? Get on-boarded with Optima, HumanaR & all our other products for your growing business',
          content4: 'Sign up for free or Contact us for assistance. ',
        },
        {
          id: 3,
          heading: 'Is there a trial period and how do I sign up?',
          content1:
            "Yes, there's a 15 day free trial period. Just enter your name, email address & password details and you're good to go.",
          content2: 'Sign up for free or Contact us for assistance. ',
        },
        {
          id: 4,
          heading:
            'How do I subscribe if I decide to use Cloudenly for my business?',
          content1:
            'You can subscribe to Cloudenly at your convenience, all you need to do is go to the <nuxt-link>pricing page</nuxt-link> and get started.',
          content2:
            'You can also subscribe at any stage in your trial period, you will also be re-directed to the pricing page at the end of your trial period. ',
          content3: 'Sign up for free or Contact us for assistance. ',
        },
        {
          id: 5,
          heading: 'What information do I need to sign up on Cloudenly?',
          content1:
            'Signing up on Cloudenly is easy, you can sign up with basic information about you and your business. You can always customize and update your information as you go',
          content2: 'Sign up for free or Contact us for assistance. ',
        },
        {
          id: 6,
          heading: 'Do I require IT expertise to use Cloudenly ERP?',
          content1:
            'No, you do not require IT expertise. As a SaaS service, the application is already preconfigured and fit for use for most people/organizations. In addition, the in-app user guide is designed to walk you through any additional setup that may be required.',
          content2: 'Sign up for free or Contact us for assistance. ',
        },
        {
          id: 7,
          heading: 'Does Cloudenly provide setup assistance?',
          content1:
            'Getting started on Cloudenly is so easy that you will likely not need assistance. However we have a step-by-step process to set up which you can access in our <nuxt-link to="/resources">resource library</nuxt-link> . We also have a friendly and knowledgeable support team that is here to help you.',
          url1: '',
          content2: 'Sign up for free or Contact us for assistance. ',
        },
      ],
      faqs3: [
        {
          id: 1,
          heading: 'How do I pay for my Cloudenly  subscriptions?',
          content1:
            'You can pay for your Cloudenly subscriptions in a secured way using your debit/credit card.',
          content2: 'Sign up for free or Contact us for assistance. ',
        },
        {
          id: 2,
          heading: 'What payment methods do you accept?',
          content1:
            'You can pay for your subscription using any Mastercard or Visa credit card or an debit card.',
          content2: 'Sign up for free or Contact us for assistance. ',
        },
        {
          id: 3,
          heading: 'Can I purchase services as a stand-alone product?',
          content1:
            'Yes, our products are designed for you to apply add-on applications as well as expand the number of users and customize to suite your business.',
          content2: 'Sign up for free or Contact us for assistance.',
        },
        {
          id: 4,
          heading: 'How much will my Cloudenly subscription cost?',
          content1:
            'Cloudenly pricing is built to be flexible and to suite your business needs. You can make use of our <nuxt-link to="/pricing">pricing calculator</nuxt-link> to determine the software and price that works for your business. ',
          content2: 'Sign up for free or Contact us for assistance. ',
        },
        {
          id: 5,
          heading: 'Will I be billed monthly or annually?',
          content1:
            'With Cloudenly, the power is in your hands, you can choose the billing method that is most convenient for you and your business, click here to get started. ',
          content2: 'Sign up for free or Contact us for assistance. ',
        },
      ],

      faqs4: [
        {
          id: 1,
          heading:
            'Can I migrate my old or historical data into Cloudenly from another platform?',
          content1:
            'Cloudenly presently supports the migration of your employee data, CRM and Product catalogue using our customized CSV. template.',
          content2: 'Sign up for free or Contact us for assistance. ',
        },
        {
          id: 2,
          heading: 'Where is my data stored when I use Cloudenly services?',
          content1:
            'Cloudenly is hosted on Amazon Web Service (AWS) to guarantee best-in-class cloud computing and security services. However, wherever local regulation requires it, data would be stored locally.',
          content2: 'Sign up for free or Contact us for assistance. ',
        },
        {
          id: 3,
          heading: 'Will my data be private and safe?',
          content1:
            'We are committed to safeguarding your personal data and we have put in place adequate security measures to ensure that personal data we collect is not altered, accessed without authorization or lost. The personal data we collect are only accessed to the extent mandated by law.',
          content2: 'We ensure data privacy and security by:',
          content3: '• Making sure that access controls are in place',
          content4: '• Installing anti-virus software on our servers',
          content5:
            '• Continuously accessing internal risks and performing compliance audits',
          content6:
            '• Testing our security controls, including external audits on a regular basis ',
          content7:
            '• Providing training on data security and privacy to our employees.',
          content8: 'Sign up for free or Contact us for assistance. ',
        },
        {
          id: 4,
          heading: 'What levels of security exist on Cloudenly?',
          content1:
            'Cloudenly is designed to ensure the highest standard of security by incorporating:',
          content2: '• Encrypted password algorithm',
          content3: '• Security questions',
          content4: '• Two-factor authentication',
          content5: '• Ring-fencing',
          content6: '• Users, role-based access controls and privileges',
          content7: 'Sign up for free or Contact us for assistance. ',
        },
        {
          id: 5,
          heading: 'What happens to my data if I cancel?',
          content1:
            "If you decide to cancel during the free 15 day trial, we will delete all traces of your data from our servers immediately. When it's gone, it's gone - so before you cancel, make sure you've saved all the reports you want to keep.",
          content2:
            "If you're a paying subscriber, you will have access to your data for a 90 days period post cancellation, after which we'll delete all your data from our servers.",
          content3: 'Sign up for free or Contact us for assistance. ',
        },
        {
          id: 6,
          heading: 'Can I download a copy of my data?',
          content1:
            'Yes, Cloudenly allows you to export your data at any point in CSV. template',
          content2: 'Sign up for free or Contact us for assistance. ',
        },
      ],

      faqs5: [
        {
          id: 1,
          heading: "Are Cloudenly's products scalable?",
          content1:
            'Cloudenly products are designed for entrepreneurs, small, medium and large enterprises; and built to scale seamlessly as your business grows.',
          content2: 'Sign up for free or Contact us for assistance. ',
        },
        {
          id: 2,
          heading: 'Can I access Cloudenly on my mobile phone or tablet?',
          content1:
            'Cloudenly can be accessed from any web enabled mobile device with a web browser as long as you have your username and password.',
          content2: 'Sign up for free or Contact us for assistance. ',
        },
        {
          id: 3,
          heading: 'Can I add multiple users to my Cloudenly account?',
          content1:
            'Yes, you can add multiple users to your account. With Cloudenly, the power is in your hands and you can always customize to suite your business.',
          content2: 'Sign up for free or Contact us for assistance. ',
        },
      ],
      faqs6: [
        {
          id: 1,
          heading: 'How am I supported when I use Cloudenly?',
          content1:
            'We provide online support as part of your Cloudenly subscription. You can also access Cloudenly support through any of the following channels:',
          content2: '• Resource Library',
          content3: '• Sales Support',
          content4: '• Customer Support',
          content5: '• Technical Support',
          content6: '• Partner Network',
          content7: 'Sign up for free or Contact us for assistance. ',
        },
        {
          id: 2,
          heading: 'What type of support can I get from the Partners Network?',
          content1:
            'The partners are independent, but authorized agents. Depending on the profile of the Partner, they may provide pre-sales, onboarding, training platform and post-sales support. Some are qualified and certified subject matter experts capable of providing business consulting and advisory services for your business.',
          content2:
            'You can find an expert across the areas covered by the Cloudenly workflow platform as well as for other business needs.',
          content3:
            '<nuxt-link to="/talk-to-an-expert">Talk to an expert today</nuxt-link>.',
          content4: 'Sign up for free or Contact us for assistance. ',
        },
        {
          id: 3,
          heading: 'Do I have to pay for Partner support?',
          content1:
            'It depends on the type of support required. Partners would typically not charge for pre-sales and onboarding, but may ask for a fee when they offer post-sales technical support. However, training, certifications, 3rd party integration and advisory services are paid services.',
          content2: 'Sign up for free or Contact us for assistance. ',
        },
      ],
    }
  },
  head() {
    return {
      title: 'Cloudenly - FAQ',
      meta: [
        {
          hid: 'Cloudenly - FAQ',
          name: ' Cloudenly - FAQ',
          content: 'Frequently Asked Questions',
        },
      ],
    }
  },
}
</script>

<style scoped>
* {
  font-family: GalanoGrotesque-Medium;
  color: #343434;
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
  font-size: 15px;
  text-align: center;
  margin: auto;
  color: #fff;
}

.banner {
  max-width: 100%;
  padding: 8rem 0 7rem 0;
  margin-top: 5rem;
  text-align: center;
  background-image: url('~assets/rectangle3.jpg');
  background-repeat: no-repeat;
  background-size: 100% 100%;
  color: white;
}

@media (max-width: 728px) {
  /* .your-subscription-code {
        width: 10%;
    } */
  .add-more-attachments-hr {
    display: none;
  }
  .banner-p {
    font-size: 14px;
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
