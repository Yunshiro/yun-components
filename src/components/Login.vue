<template>
  <!-- font style, google font -->
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com">
  <link href="https://fonts.googleapis.com/css2?family=Poetsen+One&family=ZCOOL+KuaiLe&display=swap" rel="stylesheet">

  <div class="login-container">
    <h2>{{ titleText }}</h2>
    <form action="" class="login-form">
      <div class="input-bar">
        <label for="username">{{ usernameText }}</label>
        <input type="text" id="username" required>
      </div>
      <div class="input-bar">
        <label for="password">{{ passwordText }}</label>
        <input type="password" id="password" required>
      </div>
      <button type="submit">{{ loginText }}</button>
      <a :href=url>{{ registerText }}</a>
    </form>
  </div>
</template>
 
<script setup lang='ts'>
// define props, set the label and button text
defineProps(
  {
    titleText: String,
    usernameText: String,
    passwordText: String,
    loginText: String,
    registerText: String,
    url: String
  }
)
</script>
 
<style scoped>
.login-container {
  font-family: "ZCOOL KuaiLe", sans-serif;


  backdrop-filter: blur(10px);

  background: rgba(255, 255, 255, 0);
  padding: 20px;
  width: 300px;
  border: 1px solid;
  border-radius: 8px;
  box-shadow: 0 0 10px rgba(93, 90, 90, 0.5);
}

.login-container h2 {
  margin-bottom: 20px;
  color: rgb(197, 197, 225);
  font-family: "ZCOOL KuaiLe", sans-serif;
}

.login-container button {
  font-family: "ZCOOL KuaiLe", sans-serif;

  width: 100%;
  padding: 10px;
  border: none;
  background-color: rgb(206, 206, 247);
  border-radius: 5px;
  font-size: 17px;
}

.login-container button:hover {
  box-shadow: 0 0 16px rgb(118, 118, 221);
}

.login-container button:hover {
  background-color: rgb(118, 118, 221);
  cursor: pointer;
}

.login-container a {
  color: rgb(197, 197, 225);
}

.input-bar {
  margin-bottom: 15px;
  text-align: left;
}

.input-bar label {
  display: block;
  margin-bottom: 5px;
  color: rgb(197, 197, 225);
  font-weight: 900;
}

.input-bar input {
  width: 100%;
  border: 1px solid rgb(247, 213, 213);
  border-radius: 5px;
  padding: 10px;
  box-sizing: border-box;
  font-size: 16px;

  font-family: "ZCOOL KuaiLe", sans-serif;

}

.input-bar input:focus {
  outline: none;
  box-shadow: 0 0 15px rgba(223, 82, 17, 0.901);
}
</style>