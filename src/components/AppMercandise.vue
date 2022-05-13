<template>
  <div class="merchandise">
      <ul>
        <li v-for="(link, index) in merchLinks" :key="`merch-${index}`">
            <img  :src="link.srcImg" alt="">
            <a :href="link.href">{{link.text}}</a>
        </li>
      </ul>
  </div>
</template>

<script>
    import one from "../assets/img/buy-comics-digital-comics.png"
    import two from "../assets/img/buy-comics-subscriptions.png"
    import tree from "../assets/img/buy-comics-merchandise.png"
    import four from "../assets/img/buy-comics-shop-locator.png"
    import five from "../assets/img/buy-dc-power-visa.svg"
export default {
    data(){
        return{
            merchLinks:[
                {
                    text: "digital comics",
                    href: "#",
                    srcImg : one

                },
                {
                    text: "dc merchandise",
                    href: "#",
                    srcImg :four

                },
                {
                    text: "subscription",
                    href: "#",
                    srcImg : two

                },
                {
                    text: "comic shop locator",
                    href: "#",
                    srcImg :tree 

                },
                {
                    text: "dc power visa",
                    href: "#",
                    srcImg :five 

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