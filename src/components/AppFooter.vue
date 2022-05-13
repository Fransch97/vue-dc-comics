<template>
  <footer>
      <div class="footer-links">
          <div class="links-container-footer">
              <ul v-for="(obj, index) in footerLinks" :key="`footer-${index}`">
                  <li><a href="" class="title-ul"></a></li>
                  <li 
                  v-for="(obj, indexx) in obj.links" 
                  :key="`footer-${indexx}`">

                    <a href="#"></a>

                  </li>
              </ul>
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


</style>