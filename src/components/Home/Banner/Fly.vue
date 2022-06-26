<template>
  <button class="flex justify-center items-center icon-fly z-20">
    <img src="~/static/icons/paper.png" />
  </button>
</template>

<script lang="ts">
import Vue from 'vue'
export default Vue.extend({
  name: 'NuxtFly',
})
</script>

<style lang="scss" scoped>
.icon-fly {
  width: 79px;
  height: 80px;
  border-radius: 50%;
  box-shadow: 0px 4px 24px rgba(0, 0, 0, 0.3);
  background-color: #ffffff;
  @media only screen and (max-width: 767px) {
    width: 60px;
    height: 60px;
  }
}
</style>