<template>
  <div class="content">
      <div class="comic-card">
        <div class="img">
            <img :src="docs.thumb" alt="">
        </div>
        <span class="txt">{{docs.series}}</span>
      </div>
  </div>
</template>

<script>
export default {
    props:{
        docs : Object
    }
}
</script>

<style lang="scss" scoped>
@import "../assets/styles/_var.scss";
@import "../assets/styles/_content.scss";


</style>