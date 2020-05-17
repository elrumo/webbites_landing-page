<template>
  <div class="logoImg">
      <img v-if="color == 'white'" src="@/assets/landingPage/WebBites_white.svg"/>
      <img v-if="color == 'blue'" src="@/assets/landingPage/WebBites.svg"/>
  </div>
</template>

<script>
export default {
    name:"Logo",
    props:{
      color:{}
    },
    mounted(){
    }
}
</script>

<style>
  .logoImg{
    height: 100%;
    height: fit-content;
  }
  .logoImg img{
    height: fit-content;
    width: auto !important;
    color: var(--darkBlue)
  }
</style>