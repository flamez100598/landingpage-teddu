<template>
  <div class="flex w-full justify-center partnership">
    <div class="flex w-full justify-end partnership-container">
      <div class="flex flex-col lg:flex-row w-full partnership-container__body">
        <div class="left">
          <div class="title">Partnership</div>
          <div class="description">
            We choose to work with like-minded partners who share the same vision and purpose, to achieve business goal of all parties.
          </div>
        </div>
        <div class="right">
          <img src="~/static/images/img-partnership.png" class="w-full" />
        </div>
      </div>
    </div>
  </div>
</template>

<script lang="ts">
import Vue from 'vue'
export default Vue.extend({
  name: 'NuxtPartnership',
})
</script>

<style lang="scss" scoped>
.partnership {
  padding-top: 11px;
  &-container {
    max-width: 1440px;
    &__body {
      max-width: 1354px;
      @media only screen and (max-width: 1439px) {
        padding-left: 2rem;
      }
      .left {
        width: 43%;
        @media only screen and (max-width: 1023px) {
          width: 100%;
        }
        .title {
          padding-top: 150px;
          font-weight: 700;
          font-size: 66px;
          line-height: 1.1;
          letter-spacing: -0.04em;
          color: #11262e;
          @media only screen and (max-width: 1023px) {
            padding-top: 50px;
            font-size: 32px;
            line-height: 1.25;
          }
        }
        .description {
          max-width: 416px;
          padding-top: 20px;
          font-weight: 400;
          font-size: 20px;
          line-height: 1.6;
          color: #3c4352;
          @media only screen and (max-width: 1023px) {
            padding-top: 12px;
            font-size: 14px;
            line-height: 1.4;
          }
        }
      }
      .right {
        width: 57%;
        padding-right: 24px;
        @media only screen and (max-width: 1023px) {
          width: 100%;
          padding-top: 22px;
        }
      }
    }
  }
}
</style>