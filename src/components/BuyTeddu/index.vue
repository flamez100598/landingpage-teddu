<template>
    <div class="flex w-full justify-center main-buy-teddu">
        <div class="flex flex-col w-full relative buy-teddu-container"> 
            <div class="background">
                <img
                src="~/static/images/bg-buy-teddu.png"
                class="w-full absolute top-0 left-0 desktop"
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
                                <div class="select flex">
                                    <span>BNB</span>
                                    <img class="icon-dropdown" src="~/static/icons/icon-dropdown.png" />
                                </div>
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
                        <div class="teddu-coin flex flex-col"> 
                            <div class="select-coin">
                                <img src="~/static/icons/bnb.png" />
                                <div class="select flex">
                                    <span>BNB</span>
                                    <img class="icon-dropdown" src="~/static/icons/icon-dropdown.png" />
                                </div>
                            </div>
                            <div class="input"> 
                                <input type="text" />
                            </div>
                            <div> 

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
        height: 960px;
    }
    .main-content {
        width: 57%;
        margin: 0 auto;
        border: 4px solid #000000;
        border-radius: 32px;
        position: absolute;
        top: 17%;
        position: absolute;
        left: 0;
        right: 0;
        margin-left: auto;
        margin-right: auto;
        .form-convert {
            padding: 90px 58px;
            background: linear-gradient(0deg, #EFE9E0 -39.29%, #FFFFFF 128.89%);
            border: 8px solid #FFFFFF;
            box-shadow: 0px 24px 12px rgb(0 0 0 / 10%);
            border-radius: 16px;
            margin: 10px;
            position: relative;
            .title-form {
                position: absolute;
                top: -50px;
                left: 0;
                right: 0;
                margin-left: auto;
                margin-right: auto;
                width: 50%;
            }
            .select-coin {
                display: flex;
                align-items: center;
                img {
                    width: 70px;
                    height: 70px;
                    z-index: 1;
                }
                .select {
                    background: #E2CEAE;
                    border-radius: 8px;
                    padding: 10px 30px;
                    position: relative;
                    left: -20px;
                    z-index: 0;
                    font-weight: 400;
                    font-size: 32px;
                    line-height: 38px;
                    color: #050505;
                    width: 230px;
                }
                .icon-dropdown {
                    position: absolute;
                    right: 5px;
                    top: 6px;
                    width: 46px;
                    height: 46px;
                }
                .input-select {
                    color: #000000;
                    display: block;
                    width: 100%;
                    padding: 2px 25px 2px 2px; 
                    border: none; 
                    background: url("~/static/icons/icon-dropdown.png") right center no-repeat; 
                }
            }
        }
    }
}
</style>