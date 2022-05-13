<template>
  <div class="merchandise">
      <ul>
        <li v-for="(link, index) in merchLinks" :key="`merch-${index}`">
            <img  :src=" '../assets/img/' + link.srcImg" alt="">
            <a :href="link.href">{{link.text}}</a>
        </li>
      </ul>
  </div>
</template>

<script>
export default {
    data(){
        return{
            merchLinks:[
                {
                    text: "digital comics",
                    href: "#",
                    srcImg : "buy-comics-digital-comics.png"

                },
                {
                    text: "dc merchandise",
                    href: "#",
                    srcImg : "buy-comics-merchandise.png"

                },
                {
                    text: "subscription",
                    href: "#",
                    srcImg : "buy-comics-subscriptions.png"

                },
                {
                    text: "comic shop locator",
                    href: "#",
                    srcImg : "buy-comics-shop-locator.png"

                },
                {
                    text: "dc power visa",
                    href: "#",
                    srcImg : "buy-dc-power-visa.svg"

                }
            ]
        }
    }

}
</script>

<style lang="scss" scoped>
@import "../assets/styles/_global.scss";
@import "../assets/styles/_mixin.scss";
@import "../assets/styles/_merchandise.scss";
</style>