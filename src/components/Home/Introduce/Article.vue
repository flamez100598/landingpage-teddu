<template>
  <div class="article">
    <div class="article-body">
      <div class="title">{{ title }}</div>
      <div class="content">{{ content }}</div>
      <div class="learn-more">
        <a :href="url" target="_blank">Learn More</a>
      </div>
    </div>
  </div>
</template>

<script lang="ts">
import Vue from 'vue'
export default Vue.extend({
  name: 'NuxtArticle',
  props: {
    title: {
      type: String,
      default: '',
    },
    content: {
      type: String,
      default: '',
    },
    url: {
      type: String,
      default: '',
    },
  },
})
</script>

<style lang="scss" scoped>
.article {
  filter: drop-shadow(0px 4px 16px rgba(0, 0, 0, 0.07));
  &-body {
    height: 100%;
    min-height: 250px;
    padding: 28px 24px;
    background: #ffffff;
    // box-shadow: 0px 4px 16px rgba(0, 0, 0, 0.07);
    clip-path: polygon(0% 0%, 100% 0%, 100% 85%, 85% 100%, 0% 100%);
    @media only screen and (max-width: 767px) {
      padding: 20px 20px 24px 20px;
      min-height: 178px;
    }
    .title {
      font-weight: 700;
      font-size: 28px;
      line-height: 36px;
      color: #11262e;
      @media only screen and (max-width: 767px) {
        font-size: 18px;
        line-height: 36px;
      }
    }
    .content {
      padding-top: 12px;
      font-weight: 400;
      font-size: 14px;
      line-height: 21px;
      color: #3c4352;
      @media only screen and (max-width: 767px) {
        font-size: 12px;
        line-height: 18px;
        padding-top: 8px;
      }
    }
    .learn-more {
      padding-top: 20px;
      color: #00704e;
      font-weight: 600;
      font-size: 18px;
      line-height: 22px;
      text-transform: capitalize;
      @media only screen and (max-width: 767px) {
        font-size: 14px;
        line-height: 17px;
        padding-top: 12px;
      }
    }
  }
}
</style>