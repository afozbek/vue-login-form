<template>
  <div id="app">
    <div class="m-flexContainer">
      <img
        class="a-heroImage"
        alt="Vue logo"
        src="https://colorlib.com/etc/lf/Login_v18/images/bg-01.jpg"
      />
      <div class="m-formContainer">
        <LoginForm />
      </div>
    </div>
    <!-- <HelloWorld msg="Welcome to Your Vue.js App" /> -->
  </div>
</template>

<script>
import LoginForm from "./components/LoginForm.vue";

export default {
  name: "app",
  components: {
    LoginForm
  }
};
</script>

<style lang="scss">
/* GLOBAL SCSS IMPORT */
@import "./scss/main.scss";
</style>
