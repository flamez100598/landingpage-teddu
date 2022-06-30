<template>
  <div class="flex w-full justify-center feature-banner">
    <div class="flex w-full justify-center feature-container relative">
      <img src="~/static/images/table.png" />
    </div>
  </div>
</template>

<script>
export default {}
</script>

<style lang="scss" scoped>
.feature-banner {
  line-height: 1.6;
  .feature-container {
    max-width: 1440px;
    background-image: url(~/static/images/bg-table.png);
    background-repeat: no-repeat;
    background-size: cover;
    padding: 150px 155px 120px 155px;
  }
}
</style>