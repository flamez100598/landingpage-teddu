<template>
  <div class="card-container">
    <div class="inner-card relative">
      <div class="card-title" :class="titleRight">
        <img :src="src" alt="" />
      </div>
      <div class="card-content">
        {{ content }}
      </div>
      <div class="icon-card" :class="iconRight">
        <img :src="srcIcon" alt="" />
      </div>
    </div>
  </div>
</template>

<script>
export default {
  props: {
    src: String,
    srcIcon: String,
    content: String,
    titleRight: String,
    iconRight: String,
  },
}
</script>

<style lang="scss" scoped>
.card-container {
}
.inner-card {
  background-image: url(~/static/images/bg-card.png);
  background-position: center;
  background-size: contain;
  background-repeat: no-repeat;
  max-width: 779px;
  height: 325px;
  color: #000000;
  font-size: 15px;
  padding: 0 20px;
  .card-title {
    position: absolute;
    top: -35px;
    img {
      width: 80%;
    }
  }
  .title-right {
    right: -100px;
  }
  .card-content {
    width: 80%;
    margin: 0 auto;
    text-align: left;
    padding-top: 60px;
  }
  .icon-card {
    position: absolute;
    bottom: 30px;
    z-index: 1;
  }
  .icon-right {
right: -15px;
  }
}
</style>