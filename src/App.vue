<template>
  <div>
    <Login 
      title-text="Login"
      username-text="Username"
      password-text="Password"
      login-text="Login"
      register-text="Create an Account?"
      url="#"
    ></Login>
  </div>
</template>
 
<script setup lang='ts'>
import Login from './components/Login.vue'

</script>

<style scoped>
div {
  position: relative;
  left: 290px;
  top: 100px;

}
</style>