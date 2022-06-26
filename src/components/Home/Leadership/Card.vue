<template>
  <div class="flex flex-col items-stretch card">
    <img :src="src" />
    <div class="flex flex-col h-full items-stretch card-content">
      <div class="title">
        {{ name }}
      </div>
      <div class="position">
        {{ position }}
      </div>
      <div class="description">
        {{ description }}
      </div>
      <div class="flex h-full items-end link">
        <a :href="linkedin">Linkedin</a>
      </div>
    </div>
  </div>
</template>

<script lang="ts">
import Vue from 'vue'
export default Vue.extend({
  name: 'NuxtCard',
  props: {
    src: {
      type: String,
      default: '',
    },
    name: {
      type: String,
      default: '',
    },
    position: {
      type: String,
      default: '',
    },
    description: {
      type: String,
      default: '',
    },
    tiwitter: {
      type: String,
      default: '',
    },
    linkedin: {
      type: String,
      default: '',
    },
  },
})
</script>
<style lang="scss" scoped>
.card {
  background: #ffffff;
  border: 1px solid #ffffff;
  box-shadow: 0px 4px 16px rgba(0, 0, 0, 0.07);
  img {
    width: 100%;
    max-width: unset;
  }
  .card-content {
    padding: 28px 24px 20px;
    @media only screen and (max-width: 767px) {
      padding: 28px 24px 24px;
    }
    .title {
      font-weight: 700;
      font-size: 20px;
      line-height: 21px;
      color: #11262e;
    }
    .position {
      padding-top: 8px;
      color: #3c4352;
      font-weight: 500;
      font-size: 12px;
    }
    .description {
      padding-top: 12px;
      color: #3c4352;
      font-weight: 400;
      font-size: 12px;
    }
    .link {
      a {
        width: 76px;
        height: 28px;
        display: flex;
        justify-content: center;
        align-items: center;
        margin-right: 12px;
        margin-top: 20px;
        background: linear-gradient(180deg, #1ba662 0%, #045e39 100%);
        border-radius: 4px;
        font-weight: 600;
        font-size: 12px;
        color: white;
        white-space: nowrap;
        @media only screen and (max-width: 767px) {
          width: 65px;
          height: 24px;
        }
      }
    }
  }
}
</style>