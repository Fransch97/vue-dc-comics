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


export default {
  components: { AppHeader, AppMain, AppMercandise, AppFooter, AppSocial },
  data() {
    return {
    }
  },
mounted() {
},
}
</script>

<style lang="scss" >
@import "./assets/styles/_var.scss";
@import "./assets/styles/_global.scss";
@import "./assets/styles/_mixin.scss";




</style>
