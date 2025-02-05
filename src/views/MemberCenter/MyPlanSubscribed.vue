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
  /* max-width: 800px; */
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
.mainTitle {
  margin: 50px 0;
  display: block;
  max-width: 100%;
}

.plan {
  margin: 50px 0;
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
  display: flex;
  align-items: center;
  justify-content: flex-end;
  gap: 10px;
}
.btnKey-L {
  margin: 30px 0;
  display: flex;
  justify-content: center;
  width: fit-content;
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
          <img :src="mainTitle" class="mainTitle" alt="title" />
        </div>
        <div class="user-details">
          <div class="detail-item">
            <img :src="feather" alt="feather" />
            <span class="label">Plan</span>
          </div>
          <span class="value">Annual Subscription Plan</span>
          <div class="detail-item">
            <img :src="feather" alt="feather" />
            <span class="label">Subscription Period</span>
          </div>
          <span class="value">From July 22, 2024, to July 21, 2025</span>
          <div class="detail-item">
            <img :src="feather" alt="feather" />
            <span class="label">Next Renewal Date</span>
          </div>
          <span class="value">July 22, 2025</span>
        </div>
        <div class="cancel">
          <p>Cancel Subscription</p>
          <div class="i">
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
        <div class="content-center">
          <img :src="plan" class="plan" alt="plan" />
          <div class="btnKey-L dark">
            <p>CHANGE</p>
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
        </div>
      </div>
    </div>
  </div>
</template>
<script setup>
import feather from "@/assets/img/feather.svg";
import Logo from "@/assets/img/logo.svg";
import mainTitle from "@/assets/img/maintitle.svg";
import plan from "@/assets/img/plan.svg";
</script>
