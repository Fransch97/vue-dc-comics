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

nav{
    @include flexCen();
    align-items: stretch;
    width: 70%;
    margin: auto;
    justify-content: space-between;
//logo
    .logo{
        padding: 20px 0;
    }
    //links
    ul{ 
        @include flexCen();
        align-items: stretch;
        //li
        li{
            @include flexCen();
            margin: 0 10px;
            border-bottom: 5px solid white;
            &.active{border-bottom: 5px solid #0c7cec; }
            &.active a{
                color:#0c7cec
            }
            a{
                text-decoration: none;
                text-transform: uppercase;
                font-weight: bold;
                color: #494949;
                font-size: 14px;
            }
        }
    }
}

</style>