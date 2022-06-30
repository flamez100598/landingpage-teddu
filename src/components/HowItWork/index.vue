<template>
  <div class="flex w-full justify-center works">
    <div class="flex w-full justify-start works-container">
      <div
        class="flex flex-col lg:flex-row w-full works-container__body relative"
      >
        <div class="title absolute">
          <Title :title="'How it works'" />
        </div>
        <div class="left">
          <Card
            :src="require('~/static/images/how-it-work-title1.png')"
            :src-icon="require('~/static/icons/teddy-girl.png')"
            :content="'The Teddinu Risk Free Value (RFV) plays a critical role in the Auto-Staking Protocol. It is a separate wallet that collects funds to support and stability the Liquidity pool. This is particularly useful in the event of a sharp sell-off that might drain a liquidity pool. This can cause problems because liquidity is what allows the buying and selling of the $TEDDINU token. The RFV provides a liquidity reserve and prevents this from happening during a sharp sell-off.'"
          />
          <div class="pt-50">
            <Card
              :src="require('~/static/images/how-it-work-title3.png')"
              :content="'2% of all $TEDDINU traded are burnt in The Fire Pit. The more that is traded, the more get put into the fire causing the fire pit to grow in size, larger and larger through self fulfilling Auto-Compounding, reducing the circulating supply and keeping the Inu Base protocol stable. Transfer ownership of Fire Pit wallet address to Binance Deployer. Given their reputation, we hope the Binance Ecosystem will help the Inu Base Protocol grow stronger and more secure.'"
            />
          </div>
        </div>
        <div class="right">
          <Card
            :title-right="'title-right'"
            :src="require('~/static/images/how-it-work-title2.png')"
            :content="'The Treasury plays a very important role in Teddinu protocol. It provides three extremely critical functions for the growth and sustainability of $TEDDINU The treasury functions as additional financial support for the RFV. This additional support can become important in the event of an extreme price drop of the $TEDDINU token or unforeseen black-swan event. It helps to establish a floor value for the $TEDDINUB token. The treasury may also be used to fund new Inu Base products, services, and projects that will expand and provide more value to the Teddinu community as well as providing funding for marketing.'"
          />
          <div class="pt-50">
            <Card
              :title-right="'title-right'"
              :icon-right="'icon-right'"
              :src="require('~/static/images/how-it-work-title4.png')"
              :src-icon="require('~/static/icons/teddy-girl-dance.png')"
              :content="'Every 48 hours, the Teddinu Auto-Liquidity Provide Feature will inject automated liquidity into the market. On each buy or sell order there is a tax fee (2% Buy and 5% Sell) that automatically gets stored into an Auto-LP wallet and built into our protocol\'s smart contract. This mechanism automatically converts 50% of the amount of $INUB stored in the wallet into BNB at the current market rate. The remaining 50% of $TEDDINU in the Auto-LP wallet will be used for the $INUB side of liquidity, establishing an equal 50/50 weighting of TEDDINU/BNB.'"
            />
          </div>
        </div>
        <div class="absolute icon-center">
          <img src="~/static/icons/teddy-hat.png" alt="" />
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import Card from './Card.vue'
import Title from '~/common/Title.vue'
export default {
  components: { Title, Card },
}
</script>

<style lang="scss" scoped>
.works {
  height: 830px;
  background: linear-gradient(
    360deg,
    rgba(197, 109, 7, 0.4) -60.21%,
    rgba(32, 24, 17, 0.62) 92.03%
  );
  &-container {
    max-width: 1440px;
    &__body {
      background-image: url(~/static/images/bg-work.png);
      background-position: center;
      background-size: contain;
      background-repeat: no-repeat;
      @media only screen and (max-width: 1439px) {
        padding-left: 2rem;
      }
      .title {
        font-size: 40px;
        line-height: 48px;
        text-align: center;
        text-transform: uppercase;
        left: 0;
        right: 0;
        margin-left: auto;
        margin-right: auto;
      }
      .left {
        width: 50%;
        text-align: center;
        display: flex;
        align-items: center;
        justify-content: flex-end;
        flex-direction: column;
        text-align: center;
      }
      .right {
        width: 50%;
        text-align: center;
        display: flex;
        align-items: center;
        justify-content: flex-end;
        flex-direction: column;
        padding-right: 24px;
      }
      .icon-center {
        left: 0;
        right: 0;
        margin-left: auto;
        margin-right: auto;
        top: 36%;
        img {
          margin: 0 auto;
        }
      }
    }
  }
}
.pt-50 {
  padding-top: 50px;
}
</style>