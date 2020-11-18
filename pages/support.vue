<template>
  <div>
    <AppHeader />
    <!-- Remove shadow outline to remove outlines that appears when you click on a button or input (Focus focus:shadow-outline?) === focus:outline-none -->
    <!-- Banner Starts here -->
    <section class="banner mb-8">
      <div class="content-center mr-3 ml-3">
        <h1 class="banner-h1">Submit a Support Ticket</h1>
        <div style="max-width: 550px; margin: auto">
          <p class="banner-p font-normal">
            Our technical teams are currently facing a significant increase in
            the number of support requests. You may experience a delayed
            response time as we work to address this.
          </p>
        </div>
      </div>
    </section>
    <!-- Banner Ends here -->
    <div>
      <div class="flex flex-wrap sm:px-2 lg:px-40 justify-center mt-4 mb-20">
        <div
          class="flex flex-wrap mb-3 mt-2 w-full xs:-px-8 sm:-px-8 md:px-2 lg:px-2 -mx-2"
        >
          <div class="w-full mb-4 text-left px-2 sm:mt-3">
            <div class="bottom-navigation-div">
              <h5 class="your-description font-semibold">YOUR DESCRIPTION</h5>
              <hr
                class="w-full"
                style="
                  border: 1px solid #808080;
                  margin-top: 5px;
                  margin-bottom: 10px;
                "
              />
            </div>
            <div>
              <table class="w-full">
                <tr class="w-full flex flex-col flex-no-wrap sm:table-row">
                  <td class="md:w-1/4 lg:py-5">Your Name</td>
                  <td class="md:w-3/4 lg:py-5">
                    <input
                      id="name"
                      class="border border-solid border-gray-800 rounded w-full py-2 px-3 text-gray-700 leading-tight focus:outline-none"
                      type="text"
                    />
                  </td>
                </tr>

                <tr class="w-full flex flex-col flex-no-wrap sm:table-row">
                  <td class="md:w-1/4 lg:py-5">Your Email</td>
                  <td class="md:w-3/4 lg:py-5">
                    <input
                      id="email"
                      class="border border-solid border-gray-800 rounded w-full py-2 px-3 text-gray-700 leading-tight focus:outline-none"
                      type="text"
                      required
                    />
                  </td>
                </tr>

                <tr class="w-full flex flex-col flex-no-wrap sm:table-row">
                  <td class="md:w-1/4 lg:py-5">Your Phone or Skype ID</td>
                  <td class="md:w-3/4 lg:py-5">
                    <input
                      id="phone"
                      class="border border-solid border-gray-800 rounded w-full py-2 px-3 text-gray-700 leading-tight focus:outline-none"
                      type="text"
                      required
                    />
                  </td>
                </tr>

                <tr class="w-full flex flex-col flex-no-wrap sm:table-row">
                  <td class="md:w-1/4 lg:py-5 mr-1">Enrollment Date</td>
                  <td class="md:w-3/4 lg:py-5">
                    <input
                      id="telephone"
                      class="border border-solid border-gray-800 rounded w-full py-2 px-3 text-gray-700 leading-tight focus:outline-none"
                      type="date"
                    />
                  </td>
                </tr>

                <tr class="w-full flex flex-col flex-no-wrap sm:table-row">
                  <td class="md:w-1/4 lg:py-5 mr-1">Last Contact Date</td>
                  <td class="md:w-3/4 lg:py-5">
                    <input
                      id="telephone"
                      class="border border-solid border-gray-800 rounded w-full py-2 px-3 text-gray-700 leading-tight focus:outline-none"
                      type="date"
                    />
                  </td>
                </tr>

                <tr class="w-full flex flex-col flex-no-wrap sm:table-row">
                  <td class="md:w-1/4 lg:py-5 mr-1">Copy to</td>
                  <td class="md:w-3/4 lg:py-5">
                    <input
                      id="telephone"
                      class="border border-solid border-gray-800 rounded w-full py-2 px-3 text-gray-700 leading-tight focus:outline-none"
                      type="text"
                    />
                  </td>
                </tr>
              </table>
            </div>
          </div>

          <!-- YOUR DESCRIPTION ENDS HERE -->

          <div class="w-full mb-4 text-left px-2 sm:mt-3">
            <div class="bottom-navigation-div">
              <h5 class="your-description font-semibold">
                YOUR ACCOUNT INFORMATION
              </h5>
              <hr
                class="w-full"
                style="
                  border: 1px solid #808080;
                  margin-top: 5px;
                  margin-bottom: 10px;
                "
              />
            </div>
            <div>
              <table class="w-full">
                <tr class="w-full flex flex-col flex-no-wrap sm:table-row">
                  <td class="md:w-1/4 lg:py-5 mr-1">Your Account Number</td>
                  <td class="md:w-3/4 lg:py-5">
                    <input
                      id="number"
                      class="border border-solid border-gray-800 rounded w-full py-2 px-3 text-gray-700 leading-tight focus:outline-none"
                      type="text"
                    />
                  </td>
                </tr>
                <tr class="w-full flex flex-col flex-no-wrap sm:table-row">
                  <td class="md:w-1/4 lg:py-5 mr-1">Your Product Version</td>
                  <td class="md:w-3/4 lg:py-5">
                    <input
                      id="telephone"
                      class="border border-solid border-gray-800 rounded w-full py-2 px-3 text-gray-700 leading-tight focus:outline-none"
                      type="text"
                    />
                  </td>
                </tr>
              </table>
            </div>
          </div>

          <!-- <div class="w-full mb-4 text-left px-2 sm:mt-3">
            <div class="bottom-navigation-div">
              <h5 class="your-description font-semibold">
                YOUR CLOUDENLY INSTALLATION INFORMATION
              </h5>
              <hr
                class="w-full"
                style="border: 1px solid #808080; margin-top: 5px"
              />
            </div>
            <div>
              <table class="w-full">
                <tr class="w-full flex flex-col flex-no-wrap sm:table-row">
                  <td class="md:w-1/4 lg:py-5 flex">Edition and Hosting</td>
                  <td class="md:w-3/4 lg:py-5 edition-and-hosting">
                    <div class="block mb-3">
                      <input
                        id="name"
                        class="border border-solid border-gray-800 rounded pt-20 py-2 px-3 text-gray-700 leading-tight focus:outline-none form-radio"
                        type="radio"
                        name="radio"
                        value="1"
                      /><span style="margin-left: 6px">Cloudenly Online</span>
                    </div>
                    <div class="block mb-3">
                      <input
                        id="name"
                        class="border border-solid border-gray-800 rounded py-2 px-3 text-gray-700 leading-tight focus:outline-none form-radio"
                        type="radio"
                        name="radio"
                        value="1"
                      /><span style="margin-left: 6px"
                        >Cloudenly Entreprise</span
                      >
                    </div>
                    <div class="block mb-3">
                      <input
                        id="name"
                        class="border border-solid border-gray-800 rounded py-2 px-3 text-gray-700 leading-tight focus:outline-none form-radio"
                        type="radio"
                        name="radio"
                        value="1"
                      /><span style="margin-left: 6px"
                        >Cloudenly Community</span
                      >
                    </div>
                  </td>
                </tr>

                <tr class="w-full flex flex-col flex-no-wrap sm:table-row">
                  <td class="md:w-1/4 lg:py-5 your-subscription-code sm:flex">
                    Your Subscription Code
                  </td>
                  <td class="md:w-3/4 lg:py-5">
                    <input
                      id="phone"
                      class="border border-solid border-gray-800 rounded w-full py-2 px-3 text-gray-700 leading-tight focus:outline-none"
                      type="text"
                    />
                  </td>
                </tr>

                <tr class="w-full flex flex-col flex-no-wrap sm:table-row">
                  <td class="md:w-1/4 lg:py-5">Cloudenly Version</td>
                  <td class="md:w-3/4 lg:py-5">
                    <input
                      id="number"
                      class="border border-solid border-gray-800 rounded w-full py-2 px-3 text-gray-700 leading-tight focus:outline-none"
                      type="text"
                    />
                  </td>
                </tr>
              </table>
            </div>
          </div> -->

          <div class="w-full mb-4 text-left px-2 sm:mt-3">
            <div class="bottom-navigation-div">
              <h5 class="your-description font-semibold">TICKET DESCRIPTION</h5>
              <hr
                class="w-full"
                style="border: 1px solid #808080; margin-top: 5px"
              />
            </div>
            <div>
              <table class="w-full">
                <tr class="w-full flex flex-col flex-no-wrap sm:table-row">
                  <td class="md:w-1/4 lg:py-5">Your Account Number</td>
                  <td class="md:w-3/4 lg:py-5">
                    <input
                      id="telephone"
                      class="border border-solid border-gray-800 rounded w-full py-2 px-3 text-gray-700 leading-tight focus:outline-none"
                      type="text"
                    />
                  </td>
                </tr>
                <!-- Ticket Type Starts here -->
                <tr class="w-full flex flex-col flex-no-wrap sm:table-row">
                  <td class="md:w-1/4 lg:py-5 flex">Ticket Type</td>
                  <td class="md:w-3/4 lg:py-5 edition-and-hosting">
                    <div class="block mb-3">
                      <input
                        id="name"
                        class="border border-solid border-gray-800 rounded pt-20 py-2 px-3 text-gray-700 leading-tight focus:outline-none form-radio"
                        type="radio"
                        name="radio"
                        value="1"
                      /><span style="margin-left: 6px"
                        >Technical/Commercial/Enquiry
                      </span>
                    </div>
                    <div class="block mb-3">
                      <input
                        id="name"
                        class="border border-solid border-gray-800 rounded py-2 px-3 text-gray-700 leading-tight focus:outline-none form-radio"
                        type="radio"
                        name="radio"
                        value="1"
                      /><span style="margin-left: 6px"
                        >Subscription/Billing/Payment
                      </span>
                    </div>

                    <div class="block mb-3">
                      <input
                        id="name"
                        class="border border-solid border-gray-800 rounded py-2 px-3 text-gray-700 leading-tight focus:outline-none form-radio"
                        type="radio"
                        name="radio"
                        value="1"
                      /><span style="margin-left: 6px"
                        >Configuration & Setup
                      </span>
                    </div>

                    <div class="block mb-3">
                      <input
                        id="name"
                        class="border border-solid border-gray-800 rounded py-2 px-3 text-gray-700 leading-tight focus:outline-none form-radio"
                        type="radio"
                        name="radio"
                        value="1"
                      /><span style="margin-left: 6px"
                        >Bug/incorrect behavior (without a trace back error
                        code)
                      </span>
                    </div>

                    <div class="block mb-3">
                      <input
                        id="name"
                        class="border border-solid border-gray-800 rounded py-2 px-3 text-gray-700 leading-tight focus:outline-none form-radio"
                        type="radio"
                        name="radio"
                        value="1"
                      /><span style="margin-left: 6px">Traceable Bugs </span>
                    </div>

                    <div class="block mb-3">
                      <input
                        id="name"
                        class="border border-solid border-gray-800 rounded py-2 px-3 text-gray-700 leading-tight focus:outline-none form-radio"
                        type="radio"
                        name="radio"
                        value="1"
                      /><span style="margin-left: 6px"
                        >Urgent. High. Medium. Low
                      </span>
                    </div>

                    <div class="block mb-3">
                      <input
                        id="name"
                        class="border border-solid border-gray-800 rounded py-2 px-3 text-gray-700 leading-tight focus:outline-none form-radio"
                        type="radio"
                        name="radio"
                        value="1"
                      /><span style="margin-left: 6px"
                        >Upgrade related issue
                      </span>
                    </div>

                    <div class="block mb-3">
                      <input
                        id="name"
                        class="border border-solid border-gray-800 rounded py-2 px-3 text-gray-700 leading-tight focus:outline-none form-radio"
                        type="radio"
                        name="radio"
                        value="1"
                      /><span style="margin-left: 6px"
                        >Technical, can't Say
                      </span>
                    </div>
                  </td>
                </tr>
                <!-- Ticket Type Ends here -->

                <!-- Flag Starts here -->
                <tr class="w-full flex flex-col flex-no-wrap sm:table-row">
                  <td class="md:w-1/4 lg:py-5">Flag</td>
                  <td class="md:w-3/4 lg:py-5 edition-and-hosting flex">
                    <div class="mb-3">
                      <input
                        id="name"
                        class="border border-solid border-gray-800 rounded pt-20 py-2 px-3 text-gray-700 leading-tight focus:outline-none form-radio"
                        type="radio"
                        name="radio"
                        value="1"
                      /><span style="margin-left: 6px; margin-right: 10px"
                        >Urgent
                      </span>
                    </div>
                    <div class="mb-3">
                      <input
                        id="name"
                        class="border border-solid border-gray-800 rounded py-2 px-3 text-gray-700 leading-tight focus:outline-none form-radio"
                        type="radio"
                        name="radio"
                        value="1"
                      /><span style="margin-left: 6px; margin-right: 10px"
                        >High
                      </span>
                    </div>

                    <div class="">
                      <input
                        id="name"
                        class="border border-solid border-gray-800 rounded py-2 px-3 text-gray-700 leading-tight focus:outline-none form-radio"
                        type="radio"
                        name="radio"
                        value="1"
                      /><span style="margin-left: 6px; margin-right: 10px"
                        >Medium
                      </span>
                    </div>

                    <div class="">
                      <input
                        id="name"
                        class="border border-solid border-gray-800 rounded py-2 px-3 text-gray-700 leading-tight focus:outline-none form-radio"
                        type="radio"
                        name="radio"
                        value="1"
                      /><span style="margin-left: 6px; margin-right: 10px"
                        >Low
                      </span>
                    </div>
                  </td>
                </tr>
                <!-- Flag Starts here -->

                <tr class="w-full flex flex-col flex-no-wrap sm:table-row">
                  <td class="md:w-1/4 lg:py-5 mr-1">Subject</td>
                  <td class="md:w-3/4 lg:py-5">
                    <input
                      id="text"
                      class="border border-solid border-gray-800 rounded w-full py-2 px-3 text-gray-700 leading-tight focus:outline-none"
                      type="text"
                    />
                  </td>
                </tr>

                <tr class="w-full flex flex-col flex-no-wrap sm:table-row">
                  <td class="md:w-1/4 lg:py-5 flex">Description</td>

                  <td class="md:w-3/4 lg:py-5">
                    <textarea
                      id="textfield"
                      class="w-full border border-solid border-gray-800 resize-none rounded focus:outline-none"
                      rows="5"
                    ></textarea>
                  </td>
                </tr>

                <!-- <tr class="w-full flex flex-col flex-no-wrap sm:table-row">
                  <td class="md:w-1/4 lg:py-5">Attachments</td>
                  <td class="md:w-3/4 lg:py-5">
                    <input
                      id="text"
                      class="border border-solid border-gray-800 rounded w-full py-2 px-3 text-gray-700 leading-tight"
                      type="text"
                    />
                  </td>
                </tr>

                <tr class="w-full flex flex-col flex-no-wrap sm:table-row">
                  <td class="md:w-1/4 lg:py-5"></td>
                  <td class="md:w-3/4 lg:py-5">
                    Add more attachments
                    <hr
                      class="add-more-attachments-hr w-full"
                      style="border: 1px solid #808080; margin-top: 15px"
                    />
                  </td>
                </tr> -->
              </table>
              <hr
                class="w-full"
                style="
                  border: 1px solid #808080;
                  margin-top: 1rem;
                  margin-bottom: 1rem;
                "
              />
              <div class="flex justify-end md:mt-3">
                <button
                  type="submit"
                  class="join-btn inline-block text-sm px-6 py-4 leading-none border rounded text-white hover:bg-blue-800 mt-4 lg:mt-0 shadow-md duration-200"
                >
                  Submit
                </button>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import AppHeader from './../components/header/AppHeader'
export default {
  components: {
    AppHeader,
  },
  head() {
    return {
      title: 'Cloudenly - Support',
      meta: [
        {
          hid: 'Cloudenly - Support',
          name: 'Cloudenly - Support',
          //   content: 'Tips and Tricks of Optima, Get started with Optima.',
        },
      ],
    }
  },
}
</script>

<style scoped>
.join-btn {
  color: #fff;
}

.edition-and-hosting {
  margin-top: 10px;
}
.your-description {
  font-size: 16px;
}
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
