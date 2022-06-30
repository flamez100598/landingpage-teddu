<template>
  <div class="title-container">
    <div class="relative">{{title}}
        <div class="absolute">
            <img src="~/static/icons/hat.png" alt="">
        </div>
    </div>
  </div>
</template>

<script>
export default {
    props: {
        title: String,
    }
}
</script>

<style lang="scss" scoped>

</style>