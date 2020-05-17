<template lang="html">
  <div class="footer">
    <VueMarkdown> {{ footer }} </VueMarkdown>
  </div>
</template>

<script type="text/javascript">
  import VueMarkdown from 'vue-markdown'

  export default {
    name: "LandingNavBar",
    data: function(){
      return {
        footer:"Made with ♥️ by ++[Elias](https://eliasruiz.com/)++"
      }
    },
    components:{
      VueMarkdown
    },
    methods:{
    }
  }
</script>

<style>
  .footer{
    color: black;
    position: absolute;
    text-align: center;
    padding-bottom: 50px;
    bottom: 0;
    left: 50%;
    transform: translateX(-50%)
  }
</style>
