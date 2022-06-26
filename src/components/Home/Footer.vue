<template>
  <div class="flex justify-between align-center footer">
    <div class="copy-right">
      © 2017-2022 All rights reserved. — csa.io
    </div>
    <div class="term-codition">
      <span class="policy">Privacy Policy</span>
      <span>Terms & Conditions</span>
    </div>
  </div>
</template>

<script lang="ts">
import Vue from 'vue'
export default Vue.extend({
  name: "NuxtFooter"
})
</script>
<style lang="scss" scoped>
.footer {
  background: #D8E8E2;
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