<template>
  <div class="flex justify-center contact z-20">
    <div class="flex w-full justify-end contact-container">
      <div
        class="
          flex flex-col
          lg:flex-row
          w-full
          relative
          contact-container__body
        "
      >
        <div class="flex flex-col left">
          <div class="title">Feel free to contact us</div>
          <div class="description">
            We are the team of experts that will support your business at all
            stages.
          </div>
          <div class="icon absolute">
            <img src="~/static/icons/coinFly.png" />
          </div>
          <div class="projects"></div>
        </div>
        <div class="right">
          <form>
            <div>
              <input class="input" placeholder="Enter your name" />
            </div>
            <div class="flex flex-col lg:flex-row">
              <input class="input input_first" placeholder="Enter your phone" />
              <input class="input" placeholder="Enter your e-mail" />
            </div>
            <div class="flex">
              <input
                class="input input_description"
                placeholder="Describe your situation. How can we help you?"
              />
            </div>
            <div>
              <button type="submit" class="submit-btn">Apply now</button>
            </div>
          </form>
        </div>
      </div>
    </div>
  </div>
</template>

<script lang="ts">
import Vue from 'vue'
export default Vue.extend({
  name: 'NuxtContactUs',
  data() {
    return {}
  },
})
</script>

<style lang="scss" scoped>
.contact {
  .icon {
    bottom: -32px;
    overflow: hidden;
    @media only screen and (max-width: 1023px) {
      bottom: -15px;
      left: 0;
    }
    img {
      @media only screen and (max-width: 1023px) {
        width: 60%;
      }
    }
  }
  padding-top: 91px;
  @media only screen and (max-width: 1023px) {
    padding-top: 60px;
  }
  &-container {
    max-width: 1440px;
    &__body {
      background-image: url('~static/images/banner-contact.png');
      max-width: 1354px;
      padding: 77px 83px 91px 108px;
      @media only screen and (max-width: 1023px) {
        padding: 32px 22px 149px 40px;
        margin-left: 16px;
      }
      .left {
        width: 46%;
        padding-right: 120px;
        @media only screen and (max-width: 1023px) {
          width: 100%;
        }
        .title {
          font-weight: 700;
          font-size: 66px;
          line-height: 70px;
          letter-spacing: -0.04em;
          color: #ffffff;
          @media only screen and (max-width: 1023px) {
            font-size: 32px;
            line-height: 40px;
          }
        }
        .description {
          padding-top: 22px;
          font-weight: 400;
          font-size: 20px;
          line-height: 32px;
          color: rgba(235, 235, 235, 0.7);
          @media only screen and (max-width: 1023px) {
            font-size: 14px;
            line-height: 20px;
            padding-top: 12px;
          }
        }
      }
      .right {
        width: 54%;
        @media only screen and (max-width: 1023px) {
          width: 100%;
          padding-top: 32px;
        }
        .input {
          background: #182822;
          padding: 20px;
          width: 45%;
          color: #a9b0b2;
          font-size: 20px;
          line-height: 1.2;
          font-weight: 500;
          margin-bottom: 52px;
          margin-right: 30px;
          @media only screen and (max-width: 1023px) {
            font-size: 14px;
            width: 100%;
            margin-bottom: 36px;
          }
          &_description {
            width: 100%;
          }
          &_first {
            width: 45%;
            @media only screen and (max-width: 1023px) {
              font-size: 14px;
              width: 100%;
            }
          }
        }
        .submit-btn {
          width: 210px;
          height: 60px;
          margin-top: 8px;
          background: linear-gradient(180deg, #1ba662 0%, #045e39 100%);
          border-radius: 6px;
          color: white;
          white-space: nowrap;
          font-size: 18px;
          line-height: 22px;
          font-weight: 600;
          @media only screen and (max-width: 1023px) {
            font-size: 14px;
            line-height: 17px;
            width: 154px;
            height: 40px;
          }
        }
      }
    }
  }
}
</style>