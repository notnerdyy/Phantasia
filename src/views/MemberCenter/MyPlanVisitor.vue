<style scoped>
@import "../../Assets/css/main.css";
.wrapper {
  max-width: 1440px;
  width: 100%;
  margin: 0 auto;
  padding: 5px;
  border: 10px solid $baseBlue;
  background-color: #f9faf9f2;
  background-image: none;
}
.content {
  flex: 1;
  padding: 20px;
  border: none;
}

.content-center {
  width: 100%;
  display: flex;
  flex-direction: column;
  align-items: center;
}
.title {
  font-family: "Fanwood Text";
  color: #153243;
  white-space: nowrap;
  align-items: center;
  font-size: 28px;
  margin: 36px 0;
}

.header-container {
  margin: 0 20px;
  padding: 0 20px;
  display: flex;
  justify-content: space-between;
  align-items: center;
  border: 2px solid #153243;
  margin-top: 20px;
}

.logo {
  display: flex;
  align-items: center;
  gap: 1rem;
}

.logo img {
  width: 98px;
}
.header-title {
  font-family: "Fanwood Text";
  color: #153243;
  font-weight: 400;
  white-space: nowrap;
  align-items: center;
  font-size: 28px;
}

.menu-btn {
  width: 80px;
  height: 50px;
  background: none;
  border: 1px solid #153243;
  cursor: pointer;
  position: relative;
  padding: 0;
  border-radius: 59px;
}

.hamburger {
  position: relative;
  display: block;
  width: 50px;
  height: 2px;
  background: #153243;
  margin: auto;
}

.hamburger::before,
.hamburger::after {
  content: "";
  position: absolute;
  width: 50px;
  height: 2px;
  background: #153243;
  left: 0;
}

.hamburger::before {
  top: -8px;
}

.hamburger::after {
  bottom: -8px;
}
.member-center {
  display: flex;
  margin: 0 20px 20px;
  gap: 40px;
  padding: 0 20px;
  border: 2px solid #284163;
  border-top: none;
}

.sidebar {
  width: 320px;
  height: 665px;
  border: 2px solid #284163;
  border-right: 2px solid #153243;
  border-top: none;
}

.user-info {
  text-align: center;
  .avatar-circle {
    width: 220px;
    height: 220px;
    border-radius: 50%;
    margin: 15px;
    border: 2px solid #153243;
  }

  .user-name {
    font-family: "Fanwood Text", serif;
    color: #153243;
    font-size: 24px;
  }
}

.menu-list {
  .menu-item {
    padding: 12px 15px;
    border-bottom: 1px solid #e0e0e0;
    cursor: pointer;
    font-family: "Fanwood Text", serif;

    &.active {
      color: #153243;
      font-weight: bold;
    }

    &:hover {
      background-color: #f5f5f5;
    }
  }
}
.maintitle {
  color: #eead50;
  font-size: 24px;
  font-family: "Aleo", serif;
  margin-bottom: 50px;
}
.detail {
  font-family: "Fanwood Text", serif;
  font-size: 20px;
}
.plan {
  margin: 14px 0;
  display: block;
  max-width: 100%;
}

.name {
  font-size: 60px;
  color: #284163;
  font-family: "Aleo", serif;
  margin: 50px 0 30px 0;
}

.user-details {
  margin-bottom: 30px;
  font-family: "Fanwood Text", serif;
  font-size: 20px;
  color: #153243;

  .detail-item {
    margin: 15px 0;
    border-bottom: 1px dotted #7a7a7a;

    .label {
      color: #999999;
      margin-left: 10px;
    }
  }
}
.cancel {
  font-size: 20px;
  font-family: "Fanwood Text", serif;
  color: #153243;
  text-align: right;
}
.btnKey-L {
  margin: 50px 38px;
  display: flex;
  justify-content: center;
  width: fit-content;
}

.payment-options {
  display: flex;
  /* flex-direction: column; */
  gap: 20px;
}

.payment-option {
  width: 100%;
  display: flex;
  align-items: center;
  gap: 10px;
  border-bottom: 2px solid #153243;
}

.payment-title {
  font-family: "Aleo", serif;
  font-size: 24px;
  color: #153243;
}

.credit-card-section {
  margin-top: 20px;
}
.credit-card-form {
  margin: 0 auto;
}

.form-group {
  margin-bottom: 20px;

  label {
    display: block;
    margin-bottom: 8px;
    font-family: "Fanwood Text", serif;
    color: #333;
    font-size: 16px;

    .required {
      color: #ff6b6b;
      margin-left: 4px;
    }
  }
}

.input-wrapper {
  position: relative;
  width: 100%;
  .form-input {
    width: 100%;
    padding: 12px;
    border: 1px solid #e0e0e0;
    border-radius: 4px;
    font-family: "Fanwood Text", serif;
    font-size: 16px;
    background-color: #fff;

    &::placeholder {
      color: #999;
    }
  }

  .i {
    position: absolute;
    right: 12px;
    top: 50%;
    transform: translateY(-50%);
    cursor: pointer;
    width: 24px;
    height: 24px;
    display: flex;
    align-items: center;
    justify-content: center;
  }

  .dark-view {
    width: 16px;
    height: 16px;
  }
}
.card-logos {
  margin: 50px 0;
  padding: 24px;
}
.disclaimer {
  margin: 30px 0 50px 0;
  font-family: "Fanwood Text", serif;
  font-size: 14px;
  line-height: 1.6;
  color: #153243;
  padding: 0 12px;
}
</style>

<template>
  <div class="wrapper">
    <div class="header-container">
      <div class="logo">
        <img :src="Logo" height="98px" alt="Logo" />
      </div>
      <p class="header-title">Reading is more than words</p>
      <button class="menu-btn">
        <span class="hamburger"></span>
      </button>
    </div>
    <div class="member-center">
      <!-- 左側選單 -->
      <div class="sidebar">
        <div class="user-info">
          <div class="avatar-circle"></div>
        </div>
        <div class="tab-group">
          <div class="btnTab">
            <div class="text">
              <p>Member Center</p>
            </div>
            <div class="tab-cross">
              <div class="cols">
                <span></span>
                <span></span>
              </div>
              <div class="rows">
                <span></span>
              </div>
            </div>
          </div>
          <div class="btnTab-click">
            <div class="text">
              <p>Subscription Plan</p>
            </div>
            <div class="tab-cross">
              <div class="cols">
                <span></span>
                <span></span>
              </div>
              <div class="rows">
                <span></span>
              </div>
            </div>
          </div>
          <div class="btnTab-click">
            <div class="text">
              <p>My Plan</p>
            </div>
            <div class="tab-cross">
              <div class="cols">
                <span></span>
                <span></span>
              </div>
              <div class="rows">
                <span></span>
              </div>
            </div>
          </div>
          <div class="btnTab">
            <div class="text">
              <p>Purchase history</p>
            </div>
            <div class="tab-cross">
              <div class="cols">
                <span></span>
                <span></span>
              </div>
              <div class="rows">
                <span></span>
              </div>
            </div>
          </div>
          <div class="btnTab">
            <div class="text">
              <p>My projects</p>
            </div>
            <div class="tab-cross">
              <div class="cols">
                <span></span>
                <span></span>
              </div>
              <div class="rows">
                <span></span>
              </div>
            </div>
          </div>
          <div class="btnTab">
            <div class="text">
              <p>Account Setting</p>
            </div>
            <div class="tab-cross">
              <div class="cols">
                <span></span>
                <span></span>
              </div>
              <div class="rows">
                <span></span>
              </div>
            </div>
          </div>
          <div class="btnTab">
            <div class="text">
              <p>FAQ</p>
            </div>
            <div class="tab-cross">
              <div class="cols">
                <span></span>
                <span></span>
              </div>
              <div class="rows">
                <span></span>
              </div>
            </div>
          </div>
        </div>
      </div>

      <!-- 右側內容區 -->
      <div class="content">
        <div class="content-center">
          <p class="maintitle">Subscribe Now to Unlock the Full Story!</p>
          <p class="detail">
            Subscribe to unlock the full story! Join now to enjoy every detail
            and the thrilling ending—you're just one step away!
          </p>
          <div class="btnKey-L light">
            <p>JOIN NOW</p>
            <!-- cross (icon) :內層 class 同上(內部還有其他元素不要掉了)-->
            <div class="icon-L">
              <div class="white-cross">
                <div class="cols">
                  <span></span>
                  <span></span>
                </div>
                <div class="rows">
                  <span></span>
                </div>
              </div>
            </div>
          </div>
          <img :src="step" alt="step" />
        </div>
        <div class="subscription-section">
          <h2 class="title">SUBSCRIPTION PLAN</h2>
          <div class="content-center">
            <img :src="plan" class="plan" alt="plan" />
          </div>
          <div class="payment-section">
            <h2 class="title">PAYMENT METHOD</h2>
            <div class="payment-options">
              <!-- LINE PAY -->
              <div class="payment-option">
                <div class="btnKey-L dark-border">
                  <div class="icon-L">
                    <div class="dark-cross">
                      <div class="cols">
                        <span></span>
                        <span></span>
                      </div>
                      <div class="rows">
                        <span></span>
                      </div>
                    </div>
                  </div>
                </div>
                <span class="payment-title">LINE PAY</span>
              </div>
              <!-- JKOPAY -->
              <div class="payment-option">
                <div class="btnKey-L dark-border">
                  <div class="icon-L">
                    <div class="dark-cross">
                      <div class="cols">
                        <span></span>
                        <span></span>
                      </div>
                      <div class="rows">
                        <span></span>
                      </div>
                    </div>
                  </div>
                </div>
                <span class="payment-title">JKOPAY</span>
              </div>
            </div>
            <div class="credit-card-section">
              <div class="payment-option">
                <div class="btnKey-L dark">
                  <div class="icon-L">
                    <div class="white-cross">
                      <div class="cols">
                        <span></span>
                        <span></span>
                      </div>
                      <div class="rows">
                        <span></span>
                      </div>
                    </div>
                  </div>
                </div>
                <span class="payment-title"
                  >Credit card/debit card payment</span
                >
              </div>
              <div class="card-logos">
                <img src="@/assets/img/cardlogo.svg" alt="Mastercard" />
              </div>
              <div class="credit-card-form">
                <div class="form-group">
                  <label
                    >Credit Card Number <span class="required">*</span></label
                  >
                  <div class="input-wrapper">
                    <input
                      type="text"
                      placeholder="0000 0000 0000 0000"
                      class="form-input"
                    />
                    <div class="i">
                      <div class="dark-view"></div>
                    </div>
                  </div>
                </div>

                <div class="form-group">
                  <label>Validity Period <span class="required">*</span></label>
                  <div class="input-wrapper">
                    <input type="text" placeholder="MM/YY" class="form-input" />
                    <div class="i">
                      <div class="dark-view"></div>
                    </div>
                  </div>
                </div>

                <div class="form-group">
                  <label>CVC <span class="required">*</span></label>
                  <div class="input-wrapper">
                    <input
                      type="text"
                      placeholder="Please enter"
                      class="form-input"
                    />
                    <div class="i">
                      <div class="dark-view"></div>
                    </div>
                  </div>
                </div>

                <p class="disclaimer">
                  Please note that this platform will not charge you any
                  platform transaction fees, but the credit card you use when
                  placing an order may charge you relevant fees. Please refer to
                  its relevant service policies and regulations, and report to
                  your chosen transaction service provider Get more information.
                </p>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>
<script setup>
import feather from "@/assets/img/feather.svg";
import Logo from "@/assets/img/logo.svg";
import plan from "@/assets/img/planamount.svg";
import step from "@/assets/img/step.svg";
</script>
