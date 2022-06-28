<template>
  <div class="flex justify-between align-center footer">
    <div class="copy-right">
      Copyright ©Teddynu, 2022
    </div>
    <div class="icon-contact">
      <h2><img src="~/static/icons/keep-it-touch.png" alt=""></h2>
      <div class="list-icons">
        <a v-for="(item, index) in data" :key="index" href="#" target="_blank">
          <img src="~/static/icons/keep-it-touch.png" alt="">
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
}
</style>