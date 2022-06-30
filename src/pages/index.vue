<template>
  <div class="body-container overflow-hidden">
    <Banner />
    <BuyTeddu />
    <TedduStaking />
    <Earn />
    <HowItWork />
    <Tokenomic />
    <Features />
    <Footer />
  </div>
</template>

<script lang="ts">
import Vue from 'vue'
import Banner from '~/components/Home/Banner/index.vue'
import Footer from '~/components/Home/Footer.vue'
import BuyTeddu from '~/components/BuyTeddu/index.vue'
import Features from '~/components/Features/index.vue'
import TedduStaking from '~/components/TedduStaking/index.vue'
import Earn from '~/components/Earn/index.vue'
import HowItWork from '~/components/HowItWork/index.vue'
import Tokenomic from '~/components/Tokenomic/index.vue'

export default Vue.extend({
  name: 'IndexPage',
  components: {
    Banner,
    Footer,
    BuyTeddu,
    Features,
    TedduStaking,
    Earn,
    HowItWork,
    Tokenomic
},
})
</script>

<style lang="scss" scoped>
.body-container {  background: #302B27;
}
</style>

<style lang="scss">
/* .bgvid {
  inset: 0px;
  position: fixed;
  height: 100vh;
  width: 100vw;
  max-width: 100%;
  object-fit: cover;
  z-index: -1;
  user-select: none;
} */
@font-face {
  font-family: 'Langar';
  src: url(../static/fonts/Langar-Regular.ttf);
}
@font-face {
  font-family: "Monument Extended";
  src: local("Monument Extended"),
   url(../static/fonts/MonumentExtended-Regular.otf) format("truetype");
}
.font-mehu {
  font-family: "Monument Extended";
}
.desktop {
  @media only screen and (max-width: 767px) {
    display: none;
  }
}
.mobile {
  @media only screen and (min-width: 767px) {
    display: none;
  }
}
body {
  font-family: 'Langar';
  color: #FFFFFF;
}
.btn {
  min-width: 172.73px;
  height: 44.23px;
  background: #985C23;
  color: white;
  font-weight: 400;
  font-size: 20px;
  border: 4px solid #000000;
  border-radius: 8px;
  @media only screen and (max-width: 767px) {
    min-width: 81px;
    height: 28px;
    font-size: 14px;
  }
}
</style>

<style lang="sass">
.agile
  width: 100%

  &__actions
    margin-top: 20px

  &__nav-button
    background: transparent
    border: none
    color: #ccc
    cursor: pointer
    font-size: 24px
    transition-duration: .3s

    &:hover
      color: #888

  &__dot
    margin: 0 10px

    button
      background-color: #eee
      border: none
      border-radius: 50%
      cursor: pointer
      display: block
      height: 10px
      font-size: 0
      line-height: 0
      margin: 0
      padding: 0
      transition-duration: .3s
      width: 10px

    &--current,
    &:hover
      button
        background-color: #888

// Slides styles	
.slide
  align-items: center
  color: #fff
  display: flex
  height: 300px
  justify-content: center

  h3
    font-size: 32px
    font-weight: 300

// Slides backgrounds
$colors: #f1c40f #e67e22 #e74c3c #9b59b6 #3498db #2ecc71

@for $i from 1 through length($colors)
  $color: nth($colors, $i)

  .slide--#{$i}
    background-color: $color
</style>