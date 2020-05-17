<template lang="html">
  <section class="heroIntro">
    <div class="h1_text_btn">
      <h1 class="landingPageH1"> 
        <VueMarkdown> {{ title }} </VueMarkdown>
      </h1>
      <p class="textLandingHero"> 
        <VueMarkdown> {{ paragraph }} </VueMarkdown>
      </p>
      <LandingBtn :btnText="btnText" :fontSize="'1.1rem'"/>
    </div>
    <div class="heroImgWrappwer">
      <img :src="imgPath" class="imageLeftAlign"/>
    </div>
  </section>
</template>

<script type="text/javascript">
  import LandingBtn from '@/components/LandingBtn/LandingBtn.vue'
  import VueMarkdown from 'vue-markdown'

  export default {
    name: "h1_text_btn",
    data: function(){
      return {
      }
    },
    components:{
      LandingBtn,
      VueMarkdown
    },
    props:{
      btnText: {},
      imgPath: {},
      title: {},
      paragraph: {},
    },
    mounted(){
    },
  }
</script>

<style media="screen">
  @import url("h1TextBtn.css");
</style>
