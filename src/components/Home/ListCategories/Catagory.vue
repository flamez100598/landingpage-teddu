<template>
  <div class="article">
    <div class="title flex justify-between">
      <span>{{ title }}</span>
      <span class="block md:hidden" @click="showList = !showList">
        <img v-if="showList" src="~/static/icons/icon-down.png" />
        <img v-else src="~/static/icons/icon-up.png" />
      </span>
    </div>
    <div v-if="showList" class="fade">
      <p v-for="(item, index) of data" :key="index">
        {{item}}
      </p>
    </div>
    <!-- <div class="learn-more">
      <a :href="url" target="_blank">Learn More</a>
    </div> -->
  </div>
</template>

<script lang="ts">
import Vue from 'vue'
export default Vue.extend({
  name: 'NuxtArticle',
  props: {
    title: {
      type: String,
      default: '',
    },
    data: {
      type: Array,
      default() {
        return []
      }
    },
    url: {
      type: String,
      default: '',
    },
  },
  data() {
    return {
      showList :true
    }
  }
})
</script>

<style scoped>
.article {
}
.title {
  font-weight: 700;
  font-size: 20px;
  line-height: 36px;
  color: #11262e;
  padding-bottom: 20px;
  align-items: center;
}
.content {
  padding-top: 12px;
  font-weight: 400;
  font-size: 14px;
  line-height: 21px;
  color: #3c4352;
}
.learn-more {
  padding-top: 20px;
  color: #00704e;
  font-weight: 600;
  font-size: 18px;
  line-height: 22px;
  text-transform: capitalize;
}
.fade {
  -webkit-animation-name: fade;
  -webkit-animation-duration: 0.5s;
  animation-name: fade;
  animation-duration: 0.5s;
}

@-webkit-keyframes fade {
  from {opacity: .4}
  to {opacity: 1}
}

@keyframes fade {
  from {opacity: .4}
  to {opacity: 1}
}
</style>