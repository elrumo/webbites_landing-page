<template lang="html">
  <div id="navBar" class="landingTopMenuWrapper ">
    <div class="landingTopMenu">

      <a ref="mainLogo" href="#home">
        <Logo :color="'blue'" class="verticalCentre"/>
      </a>

      <a href="#learnMore">
        <h4 class="pageTitle verticalCentre">Learn more</h4>
      </a>

      <a target="_blank" href="https://eliasruiz.com/digitalsweetness"> 
        <h4 class="pageTitle verticalCentre">Read the story</h4>
      </a>      
      
      <!-- <router-link style="text-align: right;" to="/login"> -->
        <LandingBtn style="text-align: right;" :btnText="'Signup'" :fontSize="'0.8rem'"/>
      <!-- </router-link> -->
    </div>
  </div>
</template>

<script type="text/javascript">
  import Logo from '@/components/Logo.vue'
  import LandingBtn from '@/components/LandingBtn/LandingBtn.vue'

  export default {
    name: "LandingNavBar",
    data: function(){
      return {
      }
    },
    components:{
      LandingBtn,
      Logo
    },
    mounted(){
      window.addEventListener('scroll', this.handleScroll);
    },
    destroyed(){
      window.removeEventListener('scroll', this.handleScroll);
    },
    methods:{
      // handleScroll(event){
      handleScroll(){
        var navBarClassList = document.getElementById("navBar").classList
        navBarClassList.toggle("scroll0", window.scrollY > 100 )
      }
    }
  }
</script>

<style media="screen">
  @import url("LandingNavBar.css");
</style>
