<template lang="html">
  <!-- <router-link to="/login"> -->
  <a href="/login">
    <button :style="'font-size:'+fontSize+';'" class="landingPageBtn"> {{ btnText }} </button>
  </a>
  <!-- </router-link> -->
</template>

<script type="text/javascript">
  export default {
    name: "LandingBtn",
    data: function(){
      return {
      }
    },
    props:{
      btnText: {},
      fontSize: {}
    },
    created(){
    },
  }
</script>

<style media="screen">
@import url("LandingBtn.css");
</style>
