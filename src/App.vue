<template>
  <div id="app">
    <AppHeader/>
    <AppMain/>
    <AppMercandise/>
  </div>
</template>

<script>
import AppHeader from "./components/AppHeader.vue";
import AppMain from "./components/AppMain.vue";
import AppMercandise from "./components/AppMercandise.vue";


export default {
    components: { AppHeader, AppMain, AppMercandise }
}
</script>

<style lang="scss" >
@import "./assets/styles/_var.scss";
@import "./assets/styles/_global.scss";
@import "./assets/styles/_mixin.scss";




</style>
