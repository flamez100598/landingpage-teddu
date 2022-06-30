<template>
  <div class="flex w-full justify-center partnership">
    <div class="flex w-full justify-start partnership-container">
      <div
        class="
          flex flex-col
          lg:flex-row
          w-full
          partnership-container__body
          relative
        "
      >
        <div class="title">
          <img src="~/static/icons/title-earn.png" />
        </div>
        <div class="left">
          <div>
            <img src="~/static/icons/cat.png" />
          </div>
          <div class="description">
            At the end of the year and with $100 USD of $TEDDINU invested.
          </div>
        </div>
        <div class="right relative">
          <p class="des">
            Our products are powered by DeFi and are designed to help you
            effortlessly generate cash flow from your crypto.
          </p>
          <p class="text-earn">You can earn up to</p>
          <p class="price">$1,000,2222 USD</p>
          <p class="text-small">of $TEDDINU at 1,000,2222% APY*.</p>
          <p class="text-footer">
            Earnings are calculated in a scenario where the RFV sustains the
            rebase reward for 365 days.
          </p>
          <div class="absolute button">
            <button class="btn">Start earning now</button>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>
<script>
export default {}
</script>

<style lang="scss" scoped>
.partnership {
  height: 830px;
  &-container {
    max-width: 1440px;
    background-image: url(~/static/images/bg-earn.png);
    background-position: center;
    background-size: cover;
    background-repeat: no-repeat;
    &__body {
      background-image: url(~/static/images/bg-content-earn.png);
      background-position: center;
      background-size: contain;
      background-repeat: no-repeat;
      .title {
        width: 50%;
        right: -40px;
        position: absolute;
        top: 60px;
      }
      @media only screen and (max-width: 1439px) {
        padding-left: 2rem;
      }
      .left {
        width: 50%;
        text-align: center;
        display: flex;
        align-items: center;
        justify-content: center;
        flex-direction: column;
        text-align: center;
        @media only screen and (max-width: 1023px) {
          width: 100%;
        }
        .description {
          max-width: 532px;
          font-weight: 400;
          font-size: 38px;
          line-height: 67px;
          color: #000000;
          line-height: 1.6;
          @media only screen and (max-width: 1023px) {
            padding-top: 12px;
            font-size: 14px;
            line-height: 1.4;
          }
        }
      }
      .right {
        width: 50%;
        color: #000000;
        text-align: center;
        display: flex;
        align-items: center;
        justify-content: center;
        flex-direction: column;
        padding-right: 24px;
        font-size: 24px;
        .text-earn {
          color: #985c23;
          font-size: 42px;
        }
        .price {
          color: #ffb039;
          font-size: 88px;
        }
        .text-small {
          color: #ffb039;
          font-size: 36px;
        }
        .button {
          bottom: 90px;
          button {
            font-size: 32px;
            width: 321px;
            height: 84px;
            min-width: unset;
          }
        }
        .text-footer {
          width: 100%;
          padding-top: 50px;
          font-size: 22px;
        }
        @media only screen and (max-width: 1023px) {
          width: 100%;
          padding-top: 22px;
        }
      }
    }
  }
}
</style>