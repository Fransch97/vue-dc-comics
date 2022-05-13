<template>
  <footer>
      <div class="footer-links">
          <div class="links-container-footer">
              <ul v-for="(obj, index) in footerLinks" :key="`footer-${index}`">
                  <li><a href="" class="title-li">{{obj.title}}</a></li>
                  <li 
                  class="small-li"
                  v-for="(obx, indexx) in obj.links" 
                  :key="`footer-${indexx}`">

                    <a :href="obx.href">{{obx.txt}}</a>

                  </li>
              </ul>
          </div>
          <img id="biglogo" src="../assets/img/dc-logo-bg.png" alt="">
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
                        {
                            txt:"Characters",
                            href:"#"
                        },
                        {
                            txt : "Comics",
                            href :"#"
                        },
                        {
                            txt : "Movies",
                            href :"#"
                        },
                        {
                            txt : "TV",
                            href :"#"
                        },
                        {
                            txt : "Games",
                            href :"#"
                        },
                        {
                            txt : "Videos",
                            href :"#"
                        },
                        {
                            txt : "News",
                            href :"#"
                        }
                    ]
                },
                {
                    title: "shop",
                    links:[
                        {txt:"Shop DC",href:"#"},
                       { txt: "Shop DC Collectibles",href:"#"}
                    ]
                },
                {
                    title: "dc",
                    links:[
                        {
                            txt:"Terms Of Use",
                            href: "#"
                            },
                        {
                            txt:"Privacy policy",
                            href: "#"
                            },
                        {
                            txt:"Ad Choices",
                            href: "#"
                            },
                        {
                            txt:"Advertising",
                            href: "#"
                            },
                        {
                            txt:"Jobs",
                            href: "#"
                            },
                        {
                            txt:"Subscritpions",
                            href: "#"
                            },
                        {
                            txt:"Talent Workshops",
                            href: "#"
                            },
                        {
                            txt:"CPSC Certificates",
                            href: "#"
                            },
                        {
                            txt:"Ratings",
                            href: "#"
                            },
                        {
                            txt:"Shop Help",
                            href: "#"
                            },
                        {
                            txt:"Contact Us",
                            href: "#"
                            },
                    ]
                },
                {
                    title: "sites",
                    links:[
                        {txt:"Dc",href:"#"},
                        {txt:"MAD Magazine",href:"#"},
                        {txt:"DC Kids",href:"#"},
                        {txt:"DC universe",href:"#"},
                        {txt:"DC Power Visa",href:"#"}
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
@import "../assets/styles/_footer.scss";
@import "../assets/styles/_var.scss";


</style>