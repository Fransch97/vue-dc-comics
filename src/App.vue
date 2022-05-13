<template>
  <div id="app">
    <AppHeader/>
    <AppMain/>
    <AppMercandise/>
    <AppFooter/>
  </div>
</template>

<script>
import AppHeader from "./components/AppHeader.vue";
import AppMain from "./components/AppMain.vue";
import AppMercandise from "./components/AppMercandise.vue";
import AppFooter from "./components/AppFooter.vue";


export default {
    components: { AppHeader, AppMain, AppMercandise, AppFooter }
}
</script>

<style lang="scss" >
@import "./assets/styles/_var.scss";
@import "./assets/styles/_global.scss";
@import "./assets/styles/_mixin.scss";




</style>
