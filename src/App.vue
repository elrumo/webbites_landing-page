<template>
  <div id="app">
    <AuthPage/>
  </div>
</template>

<script>
import AuthPage from './components/AuthPage/AuthPage.vue'

export default {
  name: 'app',
  components: {
    AuthPage
  }
}
</script>

<style>
  @import url("app.css");
</style>
