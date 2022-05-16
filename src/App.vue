<template>
  <div id="app">
    <AppHeader/>
    <AppMain/>
    <AppMercandise/>
    <AppFooter/>
    <AppSocial/>
  </div>
</template>

<script>
import AppHeader from "./components/AppHeader.vue";
import AppMain from "./components/AppMain.vue";
import AppMercandise from "./components/AppMercandise.vue";
import AppFooter from "./components/AppFooter.vue";
import AppSocial from "./components/AppSocial.vue";
import json from "./assets/data/dc-comics.json";


export default {
  components: { AppHeader, AppMain, AppMercandise, AppFooter, AppSocial },
  data() {
    return {
      banana : json,
    }
  },
mounted() {
  console.log(this.banana)
},
}
</script>

<style lang="scss" >
@import "./assets/styles/_var.scss";
@import "./assets/styles/_global.scss";
@import "./assets/styles/_mixin.scss";




</style>
