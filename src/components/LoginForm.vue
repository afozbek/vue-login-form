<template>
  <form class="m-loginForm">
    <h1 class="m-loginForm__desc">{{ header }}</h1>

    <div class="m-loginForm__group">
      <animated-input
        placeholder="Email"
        :showAnimation="true"
      ></animated-input>
    </div>

    <div class="m-loginForm__group">
      <animated-input
        placeholder="Password"
        :showAnimation="false"
      ></animated-input>
    </div>

    <div class="m-loginForm__group -mg-lg">
      <div class="m-loginForm__rememberWrapper">
        <custom-checkbox
          name="remember_me"
          id="remember_me"
          labelText="Remember Me"
          checkbox="✔︎"
        ></custom-checkbox>

        <a class="m-loginForm__forgotBtn" href="#">Forgot Password</a>
      </div>
    </div>

    <div class="a-showCase">
      <custom-checkbox
        name="remember_me1"
        id="remember_me1"
        labelText="Remember Me - 1"
        checkbox="✔️"
        :checked="true"
      ></custom-checkbox>

      <custom-checkbox
        name="remember_me2"
        id="remember_me2"
        labelText="Remember Me - 2"
        checkbox="✓"
        :checked="true"
      ></custom-checkbox>

      <custom-checkbox
        name="remember_me3"
        id="remember_me3"
        labelText="Remember Me - 3"
        checkbox="✔︎"
        :checked="true"
      ></custom-checkbox>
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
