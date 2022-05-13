<template>
  <header>
      <nav>
        <div class="logo">
            <img src="../assets/img/dc-logo.png" alt="">
        </div>
        <ul>
            <li v-for="(link, index)  in links" 
            :key="`nav-${index}`"
            :class="{'active': link.active}"
            >
                <a :href="link.href">{{link.text}}</a>
            </li>
        </ul>
      </nav>
  </header>
</template>

<script>
export default {
    data(){
        return{
            links:[
                {
                    text : "characters",
                    active : false,
                    href : "#"
                },
                {
                    text : "comics",
                    active : true,
                    href : "#"
                },
                {
                    text : "movies",
                    active : false,
                    href : "#"
                },
                {
                    text : "tv",
                    active : false,
                    href : "#"
                },
                {
                    text : "games",
                    active : false,
                    href : "#"
                },
                {
                    text : "collectibles",
                    active : false,
                    href : "#"
                },
                {
                    text : "videos",
                    active : false,
                    href : "#"
                },
                {
                    text : "fans",
                    active : false,
                    href : "#"
                },
                {
                    text : "news",
                    active : false,
                    href : "#"
                },
                {
                    text : "shop",
                    active : false,
                    href : "#"
                }
            ]
        }
    }
}
</script>

<style lang="scss" >
@import "../assets/styles/_mixin.scss";
@import "../assets/styles/_global.scss";
@import "../assets/styles/_header.scss";

</style>