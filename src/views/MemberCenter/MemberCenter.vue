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

.title {
  font-family: "Fanwood Text";
  color: #153243;
  white-space: nowrap;
  align-items: center;
  font-size: 28px;
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
  font-weight: 400;
  color: #153243;
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
  /* max-width: 1200px; */
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

.content {
  border: none;
  flex: 1;
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

  .detail-item {
    margin: 15px 0;
    border-bottom: 1px dotted #7a7a7a;
    color: #153243;

    .label {
      color: #999999;
      margin-left: 10px;
    }
  }
}

.subscription-box {
  background-color: #dee2e6;
  padding: 20px;
  border-radius: 8px;
  margin-bottom: 30px;

  h3 {
    color: #153243;
    margin-bottom: 15px;
    font-family: "Fanwood Text", serif;
  }

  .subscription-details {
    font-family: "Fanwood Text", serif;

    p {
      margin-bottom: 8px;
    }

    .manage-link {
      color: #153243;
      text-decoration: none;
      display: block;
      text-align: right;
      margin-top: 15px;
      display: flex;
      align-items: center;
      justify-content: right;
      gap: 10px;
    }
  }
}

.stamp-count {
  text-align: center;
  margin-top: 30px;
}
.page-link {
  text-align: right;
  display: block;
  margin-top: 15px;
  font-family: "Fanwood Text", serif;
  display: flex;
  align-items: center;
  justify-content: right;
  gap: 10px;
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
          <div class="btnTab-click">
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
          <div class="btnTab">
            <div class="text">
              <p>Draft</p>
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
        <h1 class="name">Harry Potter</h1>
        <div class="user-details">
          <div class="detail-item">
            <img :src="feather" alt="feather" />
            <span class="label">Phone Number</span>
          </div>
          <span class="value">0982644321</span>
          <div class="detail-item">
            <img :src="feather" alt="feather" />
            <span class="label">Date Of Birth</span>
          </div>
          <span class="value">1999/09/09</span>
          <div class="detail-item">
            <img :src="feather" alt="feather" />
            <span class="label">Email</span>
          </div>
          <span class="value">Service@Thame.Com</span>
        </div>

        <!-- 訂閱資訊區塊 -->
        <div class="subscription-box">
          <h3>Current Subscription</h3>
          <div class="subscription-details">
            <p>Annual Subscription Plan</p>
            <p>Subscription Period: From July 22, 2024 to June 21, 2025</p>
            <p>Next Renewal Date: June 22, 2025</p>
            <div class="manage-link">
              <p style="font-size: 20px">Manage Subscription Plans</p>
              <div class="i">
                <div class="dark-arrow"></div>
              </div>
            </div>
          </div>
        </div>

        <div class="stamp-display">
          <img :src="stamp" alt="stamp" />
          <div class="page-link">
            <p style="font-size: 20px">Go To My Page</p>
            <div class="i">
              <div class="dark-arrow"></div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>
<script setup>
import stamp from "@/assets/img/Frame 427319813.svg";
import feather from "@/assets/img/feather.svg";
import Logo from "@/assets/img/logo.svg";
</script>
