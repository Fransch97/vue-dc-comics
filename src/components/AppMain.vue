<template>
  <main>
        <AppJambo />
        <AppMainContent
        
        />
  </main>
</template>

<script>
import AppJambo from './AppJambo.vue';
import AppMainContent from './AppMainContent.vue';
import json from '../assets/data/dc-comics.json';
export default {
    components: { AppJambo, AppMainContent },
    data(){
        return{
            jsondocs : json
        }
    },
    mounted(){
        console.log(this.jsondocs)
        // v-for="(el, index) in jsondocs"
        // :key="`comics-${index}`"
    }
}
</script>

<style lang="scss" >
    
@import "../assets/styles/global";
@import "../assets/styles/_var.scss";

main{
    background: black;
}
.container-main{
    margin: auto;
    width: $conWidth;
    color: white;
}
</style>