<template>
  <div id="app">
    <AppHeader/>
    <AppMain/>
  </div>
</template>

<script>
import AppHeader from "./components/AppHeader.vue";
import AppMain from "./components/AppMain.vue";


export default {
    components: { AppHeader, AppMain }
}
</script>

<style lang="scss">
@import "./assets/styles/_var.scss";
@import "./assets/styles/_global.scss";
@import "./assets/styles/_mixin.scss";




</style>
