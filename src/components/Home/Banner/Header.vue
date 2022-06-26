<template>
  <div class="flex w-full h-full relative justify-between main-header">
    <div class="logo z-10">
      <img src="~/static/icons/logo.svg" />
    </div>
    <div class="menu-center flex z-10">
      <button class="menu-btn">Home</button>
      <button class="menu-btn">Features</button>
      <button class="menu-btn">Tokenomic</button>
      <button class="menu-btn">Contact</button>
      <button class="menu-btn">Swap</button>
      <button class="menu-btn flex items-center justify-center">
        Docs
        <img class="img-docs" src="~/static/icons/icon-dropdown.png" />
      </button>
    </div>
    <div class="main-menu flex z-10">
      <button class="move-to-earn">Contact Us</button>
    </div>
  </div>
</template>

<script lang="ts">
import Vue from 'vue'
export default Vue.extend({
  name: 'NuxtHeader',
})
</script>

<style lang="scss" scoped>
.main-header {
  background-size: cover;
  max-width: 1440px;
  .logo {
    padding-top: 37px;
    padding-left: 86px;
    @media only screen and (max-width: 767px) {
      padding-top: 16px;
      padding-left: 10px;
      max-width: 65px;
    }
  }
  .flag {
    height: 40px;
    @media only screen and (max-width: 767px) {
      height: 28px;
    }
  }
  .main-menu {
    padding-top: 28px;
    padding-right: 85px;
    font-size: 14px;
    @media only screen and (max-width: 767px) {
      padding-top: 16px;
      padding-right: 16px;
      font-size: 12px;
    }
    .menu {
      min-width: 93px;
      height: 40px;
      color: #142e38;
      border: 1px solid #142e38;
      border-radius: 4px;
      margin-left: 12px;
      font-weight: 600;
      @media only screen and (max-width: 767px) {
        min-width: 65px;
        height: 28px;
      }
      img {
        padding-right: 9px;
        @media only screen and (max-width: 767px) {
          padding-right: 4px;
        }
      }
    }
    .move-to-earn {
      min-width: 172.73px;
      height: 44.23px;
      background: #985C23;
      color: white;
      margin-left: 18px;
      font-weight: 400;
      font-size: 20px;
      border: 4px solid #000000;
      border-radius: 8px;
      @media only screen and (max-width: 767px) {
        min-width: 81px;
        height: 28px;
      }
    }
  }
}
.menu-center {
  align-items: self-end;
}
.menu-btn {
  padding: 0 30px;
  font-size: 24px;
  font-weight: 400;
  color: #FFFFFF;
  .img-docs {
    padding-left: 7px;
  }

}
</style>