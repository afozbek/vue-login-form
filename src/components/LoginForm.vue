<template>
  <form class="m-loginForm">
    <h1 class="m-loginForm__desc">{{ header }}</h1>

    <div class="m-loginForm__group">
      <animated-input placeholder="Email" :showAnimation="true"></animated-input>
    </div>

    <div class="m-loginForm__group">
      <animated-input placeholder="Password" :showAnimation="false"></animated-input>
    </div>

    <div class="m-loginForm__group -mg-lg">
      <div class="m-loginForm__rememberWrapper">
        <custom-checkbox name="remember_me" id="remember_me" labelText="Furkan" checkbox="✔︎"></custom-checkbox>

        <a class="m-loginForm__forgotBtn" href="#">Forgot Password</a>
      </div>
    </div>

    <button type="submit" class="m-loginForm__submitBtn">Login</button>
  </form>
</template>

<script>
import AnimatedInput from "./inputs/AnimatedInput.vue";
import CustomCheckbox from "./inputs/CustomCheckbox.vue";

export default {
  data() {
    return {
      email: "",
      password: "",
      rememberMe: false
    };
  },
  components: {
    animatedInput: AnimatedInput,
    customCheckbox: CustomCheckbox
  },
  props: ["header"]
};
</script>