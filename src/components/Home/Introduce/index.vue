<template>
  <div class="flex w-full justify-center introduce">
    <div
      class="
        grid grid-cols-1
        md:grid-cols-3
        w-full
        gap-10
        relative
        introduce-container
      "
    >
      <div class="bg-top" />
      <div class="bg-bottom" />
      <img class="z-10 img-bottom" src="~/static/images/coin-introduce.png" />
      <div class="big-item">
        <div class="title">What we do</div>
        <div class="description">
          With professional experience in the blockchain field, we will accompany you, from strategy to execution, to bring the best out of your crypto project.
        </div>
        <button class="flex items-center justify-center btn-show-service z-30">
          Show All Services
        </button>
      </div>
      <div
        v-for="(item, index) of data"
        :key="index"
        :class="`${item.class || ''} relative`"
      >
        <div v-if="index === 0" class="btn-fly z-10">
          <Fly />
        </div>
        <Article :title="item.title" :content="item.content" :url="item.url" />
      </div>
    </div>
  </div>
</template>

<script lang="ts">
import Vue from 'vue'
import Fly from '../Banner/Fly.vue'
import Article from './Article.vue'

export default Vue.extend({
  name: 'NuxtIntroduce',
  components: { Article, Fly },
  data() {
    return {
      data: [
        {
          title: 'PR service',
          content:
            'We plan to promote your project to the potential markets in different regions (Asia, Europe, America) to execute PR campaigns and Shilling activities to attract more traffic and leads to the project.',
          url: '',
          class: 'md:col-end-4',
        },
        {
          title: 'Digital Marketing Service ',
          content:
            'We provide effective Digital tools to optimize Digital activities as well Analytical platforms to assess the performance of any Marketing campaigns We also tailor your Website including the presence and content to match the target audience',
          url: '',
          class: 'md:col-end-3',
        },
        {
          title: 'Marketing Master Package ',
          content:
            'We provide a Master Consultation on planning your Marketing as well as an execution plan ',
          url: '',
        },
        {
          title: 'Brand Identity Package ',
          content:
            'Visual Direction and Design \nDesign your Brand Identity and provide Brand Guidelines and Materials to align your business presence on various offline and online channels ',
          url: '',
        },
        {
          title: 'Blockchain technology consulting/ Deployment pagage',
          content:
            'We do not only provide high quality solutions but also ensure complete transparency and personal approach!',
          url: '',
        },
        {
          title: 'List your exchange on different Vote channels ',
          content:
            'Those include CoinGecko and CoinMarketCap, in which we provide all the necessary conditions for listing and guide your project through bureaucratic difficulties ',
          url: '',
        },
        {
          title: 'Fundraising Consulting ',
          content:
            'We have a consultation team which is very experienced in designing a pitch deck and other materials necessary for a successful funding, including both the visual design and the content.',
          url: '',
        },
        {
          title: 'Client Acquisition',
          content:
            'With our wide network of businesses and customers in the Crypto Community such as crypto exchange, service, influencers, we can connect you with the target customers or investors. Some potential channels that we are working on are LinkedIn, Telegram, Youtube or offline channels.',
          url: '',
        },
        {
          title: 'Content planning ',
          content:
            'With experienced Content team, we can help create a Master Content plan and give consultation on the style based on our most updated research of the most effective and suitable',
          url: '',
        },
      ],
    }
  },
})
</script>
 
<style lang="scss" scoped>
.introduce {
  padding-top: 89px;
  // background: linear-gradient(180deg, #f3efe9 0%, #f5f5f5 20.53%);
  padding-bottom: 103px;
  @media only screen and (max-width: 1439px) {
    padding-left: 2rem;
    padding-right: 2rem;
  }
  @media only screen and (max-width: 767px) {
    padding-bottom: 159px;
    padding-left: 16px;
    padding-right: 19px;
    padding-top: 28px;
  }
  &-container {
    max-width: 1276px;
    .bg-top {
      position: absolute;
      width: 374px;
      height: 475px;
      top: 89px;
      left: -187px;
      background: rgba(77, 231, 120, 0.15);
      box-shadow: 10px 14px 104px rgba(0, 0, 0, 0.12);
      filter: blur(200px);
      @media only screen and (max-width: 767px) {
        display: none;
      }
    }
    .bg-bottom {
      position: absolute;
      width: 440.24px;
      height: 437px;
      right: -170px;
      bottom: -247px;

      background: #f3d8b6;
      box-shadow: 10px 14px 104px rgba(0, 0, 0, 0.12);
      filter: blur(200px);
    }
    .img-bottom {
      position: absolute;
      right: -53px;
      bottom: -177px;
      @media only screen and (max-width: 767px) {
        width: 96px;
        right: -15px;
        bottom: -190px;
      }
    }
    .big-item {
      position: absolute;
      top: 0;
      left: 0;
      width: 33.33%;
      @media only screen and (max-width: 767px) {
        position: unset;
        width: 100%;
      }
      .title {
        font-weight: 700;
        font-size: 66px;
        line-height: 1.1;
        letter-spacing: -0.04em;
        color: #11262e;
        @media only screen and (max-width: 767px) {
          font-size: 28px;
        }
      }
      .description {
        padding-top: 20px;
        font-weight: 400;
        font-size: 20px;
        line-height: 1.6;
        color: #3c4352;
        @media only screen and (max-width: 767px) {
          font-size: 14px;
          line-height: 1.4;
          width: 90%;
        }
      }
      .btn-show-service {
        margin-top: 32px;
        width: 210px;
        height: 60px;
        background: linear-gradient(180deg, #1ba662 0%, #045e39 100%);
        border-radius: 6px;
        font-weight: 600;
        font-size: 18px;
        line-height: 1.2;
        color: white;
        @media only screen and (max-width: 767px) {
          font-size: 14px;
          width: 154px;
          height: 40px;
          position: absolute;
          bottom: -87px;
          left: 0;
        }
      }
    }
    .btn-fly {
      position: absolute;
      top: -28px;
      right: -5px;
      @media only screen and (min-width: 768px) {
        display: none;
      }
    }
  }
}
</style>