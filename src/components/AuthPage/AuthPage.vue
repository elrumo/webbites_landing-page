<template lang="html">
  <div class="landingPage">
        
    <LandingNavBar/>

    <div ref="home" class="pageWrapper">
      <h1TextBtn :title="hero.title" :paragraph="hero.paragraph" :btnText="hero.btnText" :imgPath="hero.imgPath"/>
    </div>
      
      <!-- <SignIn/> -->
      <section class="blueBgContainer">
        <div class="pageWrapper">
          <div class="">
            <img class="safari wow fadeInUp" alt="" src="@/assets/landingPage/webbites_screenshot_1.jpg">
          </div>
        </div>
        <div class="blueBackground"></div>
      </section>
      
      <div ref="learnMore" id="learnMore" class="pageWrapper">
        <h1TextBtn :title="learnMore.title" :paragraph="learnMore.paragraph" :btnText="learnMore.btnText" :imgPath="learnMore.imgPath"/>
      </div>

      <div class="pageWrapper">
        <Footer/>
      </div>

  </div>
</template>

<script>
  import h1TextBtn from '@/components/h1TextBtn/h1TextBtn.vue'
  import LandingNavBar from '@/components/LandingNavBar/LandingNavBar.vue'
  import Footer from '@/components/Footer/Footer.vue'

  export default {
    name: "AuthPage",
    components: {
      h1TextBtn,
      LandingNavBar,
      Footer,
     },
     data(){
       return{
         hero:{
           title: "All your websites in one place",
           paragraph: "A new approach to bookmarking.\nSign up to the open beta for free.",
           imgPath: require('@/assets/landingPage/heroImg.svg'),
           btnText: "Signup"
         },
         learnMore:{
           title: "A work in progress",
           paragraph: "WebBites is in an early development stage. If you want to be kept updated and try the beta, click on the button bellow.",
           imgPath: require('@/assets/landingPage/workInProgress.svg'),
           btnText: "Signup"
         },
       }
     },
  }
</script>

<style lang="css" scoped>
  @import url("AuthPage.css");  
</style>
