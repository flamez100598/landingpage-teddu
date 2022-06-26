<template>
  <div class="flex justify-center sub-banner relative z-20">
    <div class="flex w-full justify-end sub-banner-container">
      <div class="flex flex-col lg:flex-row w-full sub-banner-container__body">
        <div class="flex flex-col left">
          <div class="title">From whom do we work?</div>
          <div class="description">
            We attract crypto leads to the following projects
          </div>
          <div class="projects">
            <div
              v-for="project of projects"
              :key="project"
              class="inline-block project"
            >
              {{ project }}
            </div>
          </div>
        </div>
        <div class="right">
          <img src="~/static/images/img-sub-banner.png" class="w-full" />
        </div>
      </div>
    </div>
  </div>
</template>

<script lang="ts">
import Vue from 'vue'
export default Vue.extend({
  name: 'NuxtSubBanner',
  data() {
    return {
      projects: [
        'IDO/ICO projects',
        'DeFi projects',
        'AMM & Yield farming',
        'Crypto exchanges',
        'Crypto startups',
        'Crypto Wallets',
        'Crypto service companies',
      ],
    }
  },
})
</script>

<style lang="scss" scoped>
.sub-banner {
  &-container {
    max-width: 1440px;
    &__body {
      background: #19322c;
      background-image: url('~static/images/subbanner.png');
      max-width: 1354px;
      min-height: 550px;
      padding: 67px 84px 68px 107px;
      @media only screen and (max-width: 1023px) {
        padding: 32px 16px 32px 40px;
        margin-left: 16px;
      }
      .left {
        width: 46%;
        padding-right: 20px;
        @media only screen and (max-width: 1023px) {
          width: 100%;
        }
        .title {
          font-weight: 700;
          font-size: 66px;
          line-height: 1.1;
          letter-spacing: -0.04em;
          color: #ffffff;
          @media only screen and (max-width: 1023px) {
            font-size: 32px;
          }
        }
        .description {
          padding-top: 22px;
          font-weight: 400;
          font-size: 20px;
          line-height: 1.6;
          color: rgba(235, 235, 235, 0.7);
          @media only screen and (max-width: 1023px) {
            font-size: 14px;
            padding-top: 12px;
          }
        }
        .projects {
          .project {
            padding: 7px 16px;
            margin-right: 12px;
            margin-top: 12px;
            background: linear-gradient(180deg, #1ba662 0%, #045e39 100%);
            border-radius: 4px;
            color: white;
            white-space: nowrap;
            @media only screen and (max-width: 1023px) {
              padding: 4.5px 8px;
              font-size: 12px;
              line-height: 1.25;
              margin-right: 8px;
            }
          }
        }
      }
      .right {
        width: 54%;
        @media only screen and (max-width: 1023px) {
          width: 100%;
          padding-top: 32px;
        }
      }
    }
  }
}
</style>