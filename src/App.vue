<template>
  <div id="app">
    <div class="m-flexContainer">
      <div class="a-heroImage"></div>

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
