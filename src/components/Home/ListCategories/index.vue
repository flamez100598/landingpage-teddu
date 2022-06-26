<template>
  <div class="flex w-full justify-center introduce">
    <div class="grid md:grid-cols-4 grid-cols-1 md:gap-10 gap-2 relative introduce-container">
     <Catagory :title="marketingService.title" :data="marketingService.data" /> 
     <Catagory :title="blockchainDev.title" :data="blockchainDev.data" />
     <div class="listing">
        <div class="title">Listing on Websites</div>
        <div class="title">Video Production</div>
        <Catagory :title="listingWebsite.title" :data="listingWebsite.data" />
        <div class="title">Cryptocurrency Escrow Service</div>
     </div>
     <div class="contact-us">
        <div class="title">Contact Us</div>
        <div class="flex">
          <div v-for="(item, index) of social" :key="index" class="icon">
            <a :href="index !== 2 ? item.link : 'mailto:' + item.link" >
              <img :src="item.icon" width="28px" alt="" />
            </a>

          </div>
        </div>
     </div>
    </div>
  </div>    
</template>

<script lang="ts">
import Vue from "vue"
import Catagory from "./Catagory.vue"
export default Vue.extend({
  name: "NuxtListCategories",
  components: { Catagory },
  data() {
    return {
      marketingService: {
        title: "Marketing Services",
        data: [
          "Decentralized Finance Promotion",
          "Public Relations",
          "NFT Promotion",
          "NFT Consulting",
          "Youtube Influencers",
          "Influencers on Twitter",
          "Chinese Marketing",
          "Russian Marketing",
          "Korean Marketing",
          "IEO on Exchanges"
        ]
      },
      blockchainDev: {
        title: "Blockchain Development",
        data: [
          "Blockchain Services for Your Business",
          "Website Creation",
          "DeFi Development",
          "Smart Contracts Development",
          "Polkadot Smart Contract",
          "Market Making",
          "Market Making Services",
          "Blockchain Consulting",
          "Custom Blockchain Development",
        ]
      },
      listingWebsite: {
        title: "Listing on Websites",
        data: [
          "Promo Video Creation",
          "Analytical Review",
          "Whitepaper Development"
        ]
      },
      social: 
        [
          {
            icon: require("~/static/icons/facebook.png"),
            link: "https://www.facebook.com/csa.crypto.agency/"
          },
          {
            icon: require("~/static/icons/twiter.png"),
            link: "https://twitter.com/csa_agency"
          },
          {
            icon: require("~/static/icons/mail.png"),
            link: "contact@csa.business"
          },
          {
            icon: require("~/static/icons/linkedin.png"),
            link: "https://www.linkedin.com/company/csa-crypto-solutions-agency/"
          },       
        ]
    }
  }
})
</script>
<style lang="scss" scoped>
.introduce {
  // background: #F5F5F5;
  padding-left: 2rem;
  padding-right: 2rem;
  padding-top: 62px;
  padding-bottom: 50px;
}
.title {
  font-weight: 700;
  font-size: 20px;
  line-height: 36px;
  color: #11262e;
  padding-bottom: 20px;
}
.icon {
  padding-right: 12px;
}
</style>