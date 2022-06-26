<template>
  <div class="w-full partnership">
    <div class="title">Leadership</div>
    <div
      class="
        desktop
        grid grid-cols-1
        md:grid-cols-2
        lg:grid-cols-4
        gap-10
        relative
        leadership-container
      "
    >
      <Card
        v-for="(item, index) of data"
        :key="index"
        :src="item.img"
        :name="item.fullName"
        :position="item.position"
        :description="item.description"
        :linkedin="item.linkedin"
      />
    </div>
    <agile :options="myOptions" class="mobile">
      <Card
        v-for="(item, index) of data"
        :key="index"
        :src="item.img"
        :name="item.fullName"
        :position="item.position"
        :description="item.description"
        :linkedin="item.linkedin"
      />
    </agile>
    <div></div>
  </div>
</template>

<script lang="ts">
import Vue from 'vue'
import Card from './Card.vue'

export default Vue.extend({
  name: 'NuxtLeadership',
  components: { Card },
  data() {
    return {
      myOptions: {
        navButtons: false,
        dots: true,
        // responsive: [
        //   {
        //     breakpoint: 900,
        //     settings: {
        //       navButtons: true,
        //       infinite: false,
        //     },
        //   },
        // ],
      },
      data: [
        {
          img: require('~/static/images/vlad.png'),
          fullName: 'Le Manh Duc',
          position: 'CEO',
          description:
            'With an insightful mindset, Duc can always bring a comprehensive perspective on any matter of business. Having years of experience in a variety of sectors, Duc is determined to drive your business to great success.',
          linkedin: 'https://www.linkedin.com/in/duc-le-manh/',
        },
        {
          img: require('~/static/images/luis.png'),
          fullName: 'Nguyen Ngoc Anh',
          position: 'CMO', 
          description:
            "Having a keen eye for details, Anh is capable of adding valuable aspects to a project in terms of Branding and Marketing strategies. As a good communicator, she can guide other departments with a unified approach to customers' brief.",
          linkedin: 'https://www.linkedin.com/in/ngoc-anh-nguyen-31277158/',
        },
        {
          img: require('~/static/images/ruslan.png'),
          fullName: 'Ngo Quang Anh',
          position: 'CTO',
          description:
            'Having years of experience in Software Development, Anh acquires strategic thinking and strong business acumen. He is also well-versed in current technological trends and familiar with a variety of concepts to provide sound technical leadership in all aspects of your business.',
          linkedin: 'https://www.linkedin.com/in/ngo-anh-115178135/',
        },
        {
          img: require('~/static/images/alina.png'),
          fullName: 'Pham Anh Quang',
          position: 'CCO', 
          description:
            "Quang has had many years of experience in Finance and managing enterprises, especially in Blockchain field. Hence, he possesses an extensive understanding of this industry to provide valuable input to the growth of your business.  .",
          linkedin: 'https://www.linkedin.com/in/quang-pham-76661190/',
        },
      ],
    }
  },
})
</script>

<style lang="scss" scoped>
.partnership {
  max-width: 1354px;
  padding-top: 11px;
  padding-left: 2rem;
  padding-right: 2rem;
  margin: 0 auto;
}
.title {
  padding-bottom: 36px;
  font-weight: 700;
  font-size: 66px;
  line-height: 70px;
  letter-spacing: -0.04em;
  color: #11262e;
  @media only screen and (max-width: 767px) {
    font-size: 32px;
    line-height: 40px;
    padding-bottom: 20px;
  }
}
</style>