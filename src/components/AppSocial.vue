<template>
  <div class="socialsBar">
     <div class="container">
        <div class="signup">
        <a class="sign tbn">sign-up now!</a>
      </div>
      <div class="socials">
        <span>follow us</span>
        <img v-for="(img,index) in images" :src="img" alt="" :key="`img-${index}`">
        
      </div>
     </div>
  </div>
</template>

<script>
    import imgone from "../assets/img/footer-facebook.png"
    import imgtwo from "../assets/img/footer-periscope.png"
    import imgthree from "../assets/img/footer-pinterest.png"
    import imgfour from "../assets/img/footer-twitter.png"
    import imgfive from "../assets/img/footer-youtube.png"
    

export default {
  data(){
    return{
      images:[imgone,imgtwo,imgthree,imgfour,imgfive]
    }
  }
}
</script>

<style lang="scss" scoped>
@import "../assets/styles/_global.scss";
@import "../assets/styles/_mixin.scss";
@import "../assets/styles/_social.scss";
@import "../assets/styles/_var.scss";
</style>