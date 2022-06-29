<template>
  <div class="flex justify-between align-center footer">
    <div class="copy-right">
      <div class="text-copyright">Copyright ©Teddynu, 2022</div>
    </div>
    <div class="icon-contact">
      <h2><img src="~/static/icons/keep-it-touch.png" alt=""></h2>
      <div class="list-icons flex justify-evenly">
        <a v-for="(item, index) in data" :key="index" :href="item.link" target="_blank">
          <img :src="item.icon" alt="">
        </a>
      </div>
    </div>
    <div class="img-footer">
      <img src="~/static/icons/teddy.png" alt="">
    </div>
  </div>
</template>

<script lang="ts">
import Vue from 'vue'
export default Vue.extend({
  name: "NuxtFooter",
  data() {
    return {
      data: [
        {
          link: "",
          icon: require('~/static/icons/mail.png'),
        },
                {
          link: "",
          icon: require('~/static/icons/tele.png'),
        },
        {
          link: "",
          icon: require('~/static/icons/tele.png'),
        },
        {
          link: "",
          icon: require('~/static/icons/twiter.png'),
        }
      ]
    }
  }
})
</script>
<style lang="scss" scoped>
.footer {
  background: #26201A;
  padding-left: 2rem;
  padding-right: 2rem;
  color: #0E172F;
  font-weight: 600;
  font-size: 14px;
  padding-top: 22px;
  padding-bottom: 21px;
  .policy {
    padding-right: 32px;
  }
  .list-icons {
    padding-top: 30px;
  }
  .copy-right {
    position: relative;
    font-size: 20px;
    color: #ffff;
    font-weight: 400;
    width: 20%;
  }
  .text-copyright {
    position: absolute;
    bottom: 0%;
  }
  .icon-contact {
    margin-top: 80px;
  }
}
</style>