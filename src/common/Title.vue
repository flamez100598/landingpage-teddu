<template>
  <div class="title-container">
    <div class="relative pt-50">
      <p class="font-mehu">{{ title }}<img src="~/static/icons/hat.png" alt="" /></p>
    </div>
  </div>
</template>

<script>
export default {
  props: {
    title: String,
  },
}
</script>

<style lang="scss" scoped>
.pt-50 {
  padding-top: 50px;

}
p {
  display: inline-block;
  position: relative;
  z-index: 3;
  font-size: 40px;
}
img {
  position: absolute;
  top: -25px;
  right: -60px;
  z-index: -1;
}
</style>