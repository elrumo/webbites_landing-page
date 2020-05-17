<template lang="html">
  <div class="authPageWrapper">
      <!-- <h2>Log In</h2> -->
      <div id="firebaseui-auth-container"></div>
      <div id="loader">Loading...</div>

      <div id="sign-in-status"></div>
      <div id="sign-in"></div>
      <pre id="account-details"></pre>
    </div>
</template>
<script type="text/javascript">
  export default {
    name: "SignIn",
    props:{
      folders:{},
      currentFolderProp:{},
    },
    data: function(){
      return {
        toAdd: "",
        folderToCreate: "",
        userInfo: {},
        visible: "",
      }
    },
    mounted(){
    },
  }
</script>

<style media="screen">
@import url("SignIn.css");
@import url("firebaseui.css");
</style>
