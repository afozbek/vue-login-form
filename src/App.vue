<template>
  <div id="app">
    <div class="m-flexContainer">
      <img
        class="a-heroImage"
        alt="Vue logo"
        src="https://images.unsplash.com/photo-1574648264613-6e36a94c6a71?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=500&q=60"
      />
      <div class="m-formContainer">
        <LoginForm :header="headerText" />
      </div>
    </div>
    <!-- <HelloWorld msg="Welcome to Your Vue.js App" /> -->
  </div>
</template>

<script>
import LoginForm from "./components/LoginForm.vue";

export default {
  name: "app",
  data() {
    return {
      headerText: "Login to Continue"
    };
  },
  components: {
    LoginForm
  }
};
</script>

<style lang="scss">
/* GLOBAL SCSS IMPORT */
@import "./scss/main.scss";

</style>
