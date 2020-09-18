<template>
    <div>
        <div class="sm:flex product-wrapper">
              <hr class="vertical-divider" />
              <div class="center-div-icons">
                <img src="/img/icon-right.svg" />
                <div class="horizontal-line"></div>
                <img src="/img/icon-left.svg" style="margin-left: 47px" />
              </div>
              <div class="sm:w-1/2 product-features-left flex justify-center">
                <div class="card-feature">
                  <div class="feature-header">CRM</div>
                  <div class="feature-description-left">
                    Contact Registration, Customer Engagement, Pipeline
                    Management, Loyalty & Promos
                  </div>
                  <div class="feature-icons-left flex justify-items-end">
                    <img src="/img/icon-1.svg" />
                    <img src="/img/icon-2.svg" />
                    <img src="/img/icon-3.svg" />
                    <img src="/img/icon-4.svg" />
                  </div>
                </div>
                <div class="card-feature">
                  <div class="feature-header">Supply Chain</div>
                  <div class="feature-description-left">
                    Supplier Management, Product Catalog, Price Book, Quotes and
                    Invoice Management, Multi-Outlet/Multi- Inventory
                    Operations, Inventory Valuation, Material Management.
                  </div>
                  <div class="feature-icons-left flex justify-items-end">
                    <img src="/img/icon-1.svg" />
                    <img src="/img/icon-2.svg" />
                    <img src="/img/icon-3.svg" />
                    <img src="/img/icon-4.svg" />
                  </div>
                </div>
                <div class="card-feature">
                  <div class="feature-header">Account Management</div>
                  <div class="feature-description-left">
                    Account Receivables, Account Payables, Revenue, Expense,
                    Profits & Loss, Assets & Liabilities.
                  </div>
                  <div class="feature-icons-left flex justify-items-end">
                    <img src="/img/icon-1.svg" />
                    <img src="/img/icon-2.svg" />
                    <img src="/img/icon-3.svg" />
                    <img src="/img/icon-4.svg" />
                  </div>
                </div>
                <div class="card-feature">
                  <div class="feature-header">Account Management</div>
                </div>
              </div>
              <div class="sm:w-1/2 product-features-right flex justify-center">
                <div class="card-feature">
                  <div class="feature-header">Commerce Cloud</div>
                  <div class="feature-description-right">
                    PoS, Marketplace integrations
                  </div>
                  <div class="feature-icons-right flex justify-items-end">
                    <img src="/img/icon-1.svg" />
                    <img src="/img/icon-2.svg" />
                  </div>
                </div>
                <div class="card-feature">
                  <div class="feature-header">Production Management</div>
                  <div class="feature-description-right">
                    Material Requirement Planning, Material Assembly, Job
                    Orders, Material Request, Production Management
                  </div>
                  <div class="feature-icons-right flex justify-items-end">
                    <img src="/img/icon-1.svg" />
                    <img src="/img/icon-2.svg" />
                    <img src="/img/icon-3.svg" />
                    <img src="/img/icon-4.svg" />
                  </div>
                </div>
                <div class="card-feature">
                  <div class="feature-header">
                    Finance Management (Coming Soon)
                  </div>
                  <div class="feature-description-right">
                    Expense Management, Budget Planning & Management
                  </div>
                  <div class="feature-icons-right flex justify-items-end">
                    <img src="/img/icon-1.svg" />
                    <img src="/img/icon-2.svg" />
                    <img src="/img/icon-3.svg" />
                    <img src="/img/icon-4.svg" />
                  </div>
                </div>
                <div class="card-feature">
                  <div class="feature-header">Payment</div>
                  <div class="feature-description-right">
                    Payment & collection
                  </div>
                </div>
              </div>
            </div>
    </div>
</template>
<style scoped>

/* Product Card */
.product-wrapper {
  background-color: rgb(241, 245, 251, 0.4);
  border: 5px solid #ffffff;
  border-radius: 15px;
  margin-top: 30px;
  width: 1304px;
  /* height: 792px; */
  padding: 50px 80px;
  position: relative;
}
.product-features-left {
  flex-direction: column;
  /* align-items: center; */
}
.product-features-right {
  flex-direction: column;
  /* align-items: center; */
  align-items: flex-end;
}
.card-feature {
  width: 430px;
  text-align: right;
  margin-bottom: 30px;
}
.feature-header {
  font-family: GalanoGrotesque;
  font-size: 22px;
  line-height: 26px;
  color: #031a40;
}
.feature-description-left {
  font-family: GalanoGrotesqueAlt;
  font-size: 16px;
  line-height: 19px;
  text-align: right;
  color: #343434;
  margin-top: 5px;
}
.feature-description-right {
  font-family: GalanoGrotesqueAlt;
  font-size: 16px;
  line-height: 19px;
  text-align: left;
  color: #343434;
  margin-top: 5px;
}
.feature-icons-right {
  margin-top: 15px;
}
.feature-icons-left {
  justify-content: flex-end;
  margin-top: 15px;
}
.feature-icons-left img {
  margin-left: 16px;
}
.feature-icons-right img {
  margin-right: 16px;
}
.vertical-divider {
  position: absolute;
  left: 50%;
  top: 5%;
  bottom: 5%;
  width: 4px;
  height: 90%;
  /* height: 100%; */
  background: #4c9f70;
}
.horizontal-line {
  /* width: 4px; */
  /* background: #4c9f70; */
  border-bottom: solid 4px #4c9f70;
  top: 48%;
  right: 51px;
  width: 61px;
  position: absolute;
}
.product-features-right .feature-header {
  text-align: left;
}
.center-div-icons {
  display: flex;
  width: 170px;
  position: absolute;
  top: 40%;
  left: 43.3%;
}

</style>