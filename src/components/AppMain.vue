<template>
  <main>
        <AppJambo />
        <AppMainContent/>
        <span>load more</span>

  </main>
</template>

<script>
import AppJambo from './AppJambo.vue';
import AppMainContent from './AppMainContent.vue';
export default {
    components: { AppJambo, AppMainContent },
    mounted(){
        console.log(this.jsondocs[0].series)
        
     
    }
}
</script>

<style lang="scss" scoped>
    
@import "../assets/styles/global";
@import "../assets/styles/_var.scss";

main{
    background: black;
    padding-bottom: 20px ;
    text-align: center;

}
.container-main{
    margin: auto;
    width: $conWidth;
    color: white;

}
span{
    background-color: $logoColor;
    text-transform: uppercase;
    font-weight: bolder;
    color: white;
    display: inline-block;
    padding: 10px 60px;
    margin: auto;
}
</style>