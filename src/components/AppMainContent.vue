<template>
  <div class="content">
      <AppContentCard 
      
       v-for="(el, index) in jsondocs"
            :key="`comics-${index}`"
            :docs="el"
      />
  </div>
</template>

<script>
import json from '../assets/data/dc-comics.json';
import AppContentCard from './AppContentCard.vue';
export default {
    props: {
        docs: Object
    },
    components: { AppContentCard },
    data(){
        return{
            jsondocs : json
        }
    }
}
</script>

<style lang="scss" scoped>
@import "../assets/styles/_var.scss";
@import "../assets/styles/_content.scss";


</style>