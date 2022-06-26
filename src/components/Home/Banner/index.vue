<template>
  <div class="flex w-full justify-center main-banner">
    <div class="flex flex-col w-full relative banner-container">
      <div class="background">
        <img
          src="~/static/images/bg-header.png"
          class="w-full absolute top-0 left-0 desktop"
        />
        <img
          src="~/static/images/bg-banner-top-mobile.png"
          class="w-full absolute top-0 left-0 mobile"
        />
        <img
          src="~/static/images/bg-banner-bottom-mobile.png"
          class="w-full absolute bottom-0 left-0 mobile"
        />
      </div>

      <div class="flex w-full justify-center relative">
        <Header />
      </div>

      <div class="flex w-full text-center main-content relative">
        <div class="left-banner flex flex-col justify-center">
          <div class="title-logo">
            <img src="~/static/icons/TEDDINU.svg" />
          </div>
          <div class="title-banner">
            <img src="~/static/icons/star.png" />
            <span class="text">Move-To-Earn </span>
          </div>
          <div class="title-banner">
            <img src="~/static/icons/star.png" />
              <span class="text">Auto-Staking with</span>
          </div>
          <div class="title-percent">2,033,199.56%</div>
          <div class="title-btn">
            <button class="btn btn-lanch">Launch app</button>
            <button class="btn btn-buy">Buy Teddinu</button>
          </div>
        </div>
        <div class="right-banner">
          <img src="~/static/images/banner-right.png" />
        </div>
      </div>
      <!-- <div class="btn-fly">
        <Fly />
      </div> -->
    </div>
  </div>
</template>

<script lang="ts">
import Vue from 'vue'
import Header from './Header.vue'
// import Fly from './Fly.vue'
export default Vue.extend({
  name: 'NuxtBanner',
  components: { Header },
})
</script>

<style lang="scss" scoped>
.main-banner {
  line-height: 1.6;
  .banner-container {
    max-width: 1440px;
    .main-content {
      .left-banner {
        .title-banner {
          display: flex;
          padding: 11px 5px;
          align-items: center;
          .text {       
            padding-left: 23px;
            color: #FFFFFF;
            font-size: 44px;
            font-weight: 400;
          }
        }
        .title-percent {
          text-align: left;
          color: #3DFF39;
          font-size: 100px;
        }
        .title-btn {
          text-align: left;
          .btn {
            border-radius: 12px;
            font-size: 32px;
            height: 70px;
            min-width: 240px;
          }
          .btn-buy {
            background: #5794CC;
            margin-left: 40px;
          }
        }
      }
      .right-banner {
        max-width: 618px;
        max-height: 682px;

      }
      .proposal {
        margin-top: 40px;
        min-width: 210px;
        height: 60px;
        color: white;
        border-radius: 6px;
        font-weight: 600;
        font-size: 18px;
        background: linear-gradient(180deg, #1ba662 0%, #045e39 100%);
        @media only screen and (max-width: 767px) {
          margin-top: 20px;
          min-width: 154px;
          height: 40px;
          font-size: 14px;
        }
      }
      .note {
        padding-top: 16px;
        color: #00704e;
        font-size: 18px;
        font-weight: 600;
        line-height: 22px;
        @media only screen and (max-width: 767px) {
          padding-top: 12px;
          font-size: 14px;
          line-height: 17px;
        }
      }
    }
    .name-list {
      max-width: 1440px;
      // min-width: 593px;
      // overflow: auto;
      margin-top: 210px;
      clip-path: polygon(0% 20%, 17% 20%, 21% 0%, 100% 0%, 100% 100%, 0% 100%);
      height: 89px;
      @media only screen and (max-width: 767px) {
        margin-top: 95px;
        height: 40px;
      }
      img {
        @media only screen and (max-width: 767px) {
          width: 50%;
        }
      }
    }

    .btn-fly {
      position: absolute;
      right: 39px;
      bottom: -49px;
      @media only screen and (max-width: 767px) {
        display: none;
      }
    }
  }
}
</style>