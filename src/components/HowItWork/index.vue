<template>
  <div class="card-container">
    <div class="inner-card">
        <div class="icon-card">
            <img :src="srcIcon" alt="">
        </div>
        <div class="title-card">
            <img :src="src" alt="">
        </div>
        <div>{{content}}</div>
    </div>
  </div>
</template>

<script>
export default {
 props: {
    src: String,
    srcIcon: String,
    content: String
 }
}
</script>

<style>

</style>