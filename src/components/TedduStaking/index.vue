<template>
  <div class="flex w-full justify-center teddu-banner">
    <div class="flex flex-col w-full relative teddu-container">
      <div class="background">
        <img
          src="~/static/images/bg-staking.png"
          class="w-full absolute top-0 left-0 desktop"
        />
      </div>
      <div class="flex w-full justify-center relative teddu-content-container">
        <div class="main-content relative flex align-center">
          <div class="title">
            <img src="~/static/images/title-staking.png" />
          </div>
          <div class="icon-teddu">
            <img src="~/static/icons/teddy-staking.png" />
          </div>
          <div class="text-content">
            <p class="description">
              Teddinu is a innovation DeFi protocol with All-time Highest Fixed
              APY. The reward is fixed for users that every 8 minutes, your
              assets will increase by 0.01510%. Teddinu has created a
              revolutionary decentralized financial asset, through the use of
              Auto-Staking function, Teddinu help you increase wealth more
              easily.
            </p>
            <div class="percent flex">
              <img src="~/static/icons/star-yellow.png" />
              <h2>1,000,2222%</h2>
              <img src="~/static/icons/star-yellow.png" />
            </div>
            <div class="text-yellow">Fixed Staking APY</div>
            <div class="text-center button">
              <button class="btn">Launch app</button>
            </div>
            <p class="footer-content text-center">
              Achieving financial freedom simply by holding $INUB, the protocol
              will help you do the hard part.
            </p>
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
.teddu-banner {
  line-height: 1.6;
  background: linear-gradient(360deg, rgba(197, 109, 7, 0.4) -60.21%, rgba(32, 24, 17, 0.62) 92.03%);
  .teddu-container {
    max-width: 1440px;
    .teddu-content-container {
      background-image: url(~/static/images/bg-content.png);
      background-position: center;
      background-size: contain;
      background-repeat: no-repeat;
      height: 870px;
      .main-content {
        align-items: center;
      }
      .title {
        width: 50%;
        left: 0;
        position: absolute;
        top: 70px;
      }
      .icon-teddu {
        position: absolute;
        right: 0px;
        top: -90px;
      }
      .text-content {
        width: 66%;
        margin: 0 auto;
        color: #000000;
        font-weight: 400;
        font-size: 22px;
        line-height: 33px;
        .description {
          padding: 30px;
          margin-top: 40px;
        }
        .percent {
          padding: 60px 50px;
          margin-left: 50px;
          h2 {
            font-weight: 400;
            font-size: 96px;
            color: #ffb039;
            padding: 0 40px;
          }
        }
        .text-yellow {
          color: #ffb039;
          font-weight: 400;
          font-size: 40px;
          padding: 20px 0 60px 0;
          text-align: center;
        }
        .button {
            max-width: 351px;
            margin: 0 auto;
          button {
            height: 94px;
            font-size: 36px;
            border: 4px solid #000000;
            width: 100%;
          }
        }
        .footer-content {
            margin-top: 40px;
        }
      }
    }
  }
}
</style>