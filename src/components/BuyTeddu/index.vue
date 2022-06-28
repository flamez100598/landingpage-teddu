<template>
    <div class="flex w-full justify-center main-buy-teddu">
        <div class="flex flex-col w-full relative  buy-teddu-container"> 
            <div class="background">
                <img
                src="~/static/images/bg-buy-teddu.png"
                class="w-full absolute top-0 left-0 desktop"
                />
                <img
                src="~/static/images/bg-banner-top-mobile.png"
                class="w-full absolute top-0 left-0 mobile"
                />
                <img
                src="~/static/images/bg-banner-bottom-mobile.png"
                class="w-full absolute bottom-0 left-0 mobile"
                />
            </div>
            <div class="main-content"> 
                <div class="form-convert"> 
                    <div class="title-form">
                        <img src="~/static/images/title-form-buy.png" />
                    </div>
                    <div class="flex form-table">
                        <div class="stable-coin flex flex-col"> 
                            <div class="select-coin">
                                <img src="~/static/icons/bnb.png" />
                                <span class="coin">BNB</span>
                                <img src="~/static/icons/icon-dropdown.png" />
                            </div>
                            <div class="input"> 
                                <input type="text" />
                            </div>
                            <div> 
                                
                            </div>
                        </div>
                        <div class="arrow"> 
                            <img src="~/static/icons/arrow.png" />
                        </div>
                        <div class="teddu-coin"> 
                            <div class="select-coin">
                                <img src="~/static/icons/arrow.png" />
                                <span class="coin">Teddinu</span>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div> 
    </div>
</template>

<script>
export default {

}
</script>

<style lang="scss" scoped>
.main-buy-teddu {
    .buy-teddu-container {
    max-width: 1440px;
}
}
</style>