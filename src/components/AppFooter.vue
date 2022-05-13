<template>
  <footer>
      <div class="footer-links">
          <div class="links-container-footer">

          </div>
      </div>
  </footer>
</template>

<script>
export default {
    data(){
        return{
            footerLinks:[
                {
                    title: "dc comics",
                    links:[
                        "Characters",
                        "Comics",
                        "Movies",
                        "TV",
                        "Games",
                        "Videos",
                        "News"
                    ]
                },
                {
                    title: "shop",
                    links:[
                        "Shop DC",
                        "Shop DC Collectibles",
                    ]
                },
                {
                    title: "dc",
                    links:[
                        "Terms Of Use",
                        "Privacy policy",
                        "Ad Choices",
                        "Advertising",
                        "Jobs",
                        "Subscritpions",
                        "Talent Workshops",
                        "CPSC Certificates",
                        "Ratings",
                        "Shop Help",
                        "Contact Us"
                    ]
                },
                {
                    title: "sites",
                    links:[
                        "Dc",
                        "MAD Magazine",
                        "DC Kids",
                        "DC universe",
                        "DC Power Visa"
                    ]
                }
            ]
        }
    }

}
</script>

<style lang="scss" scoped>
@import "../assets/styles/_global.scss";
@import "../assets/styles/_mixin.scss";


</style>