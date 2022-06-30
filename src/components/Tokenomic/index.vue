<template>
  <div class="flex w-full justify-center main-banner">
    <div class="flex flex-col w-full relative banner-container">
      <div class="background">
        <img
          src="~/static/images/bg-tokenomic.png"
          class="w-full absolute top-0 left-0 desktop"
        />
      </div>

      <div class="flex w-full justify-center relative">
        <Title :title="'Teddinu tokenomics explains'" />
      </div>
      <div class="flex w-full justify-center text-center bolder">
        <p class="pd-50">
          $TEDDINU is a BEP-20 token with innovation technology that rewards
          holders every 8 minutes. In InuBase Protocol, everything is
          transparent
        </p>
      </div>
      <div class="flex w-full text-center bolder pd-50">
        <img src="~/static/images/tokenomic.png" alt="" />
      </div>
    </div>
  </div>
</template>

<script lang="ts">
import Vue from 'vue'
import Title from '~/common/Title.vue'
// import Fly from './Fly.vue'
export default Vue.extend({
  name: 'NuxtBanner',
  components: { Title },
})
</script>

<style lang="scss" scoped>
.main-banner {
  line-height: 1.6;
  .banner-container {
    max-width: 1440px;
  }
  .background {
    img {
      height: 100%;
    }
  }
}
.bolder {
  z-index: 1;
}
.pd-50 {
    padding: 50px;
}
</style>