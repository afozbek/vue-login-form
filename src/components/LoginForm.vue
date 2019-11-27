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
        <div class="m-loginForm__checkboxWrapper">
          <input
            class="m-loginForm__confirm"
            v-model="rememberMe"
            type="checkbox"
            name="remember"
            id="remember"
          />

          <label class="m-loginForm__confirmLabel" for="remember">Remember Me</label>
        </div>

        <a class="m-loginForm__forgotBtn" href="#">Forgot Password</a>
      </div>
    </div>

    <button type="submit" class="m-loginForm__submitBtn">Login</button>
  </form>
</template>

<script>
import AnimatedInput from "./inputs/AnimatedInput.vue";

export default {
  data() {
    return {
      email: "",
      password: "",
      rememberMe: false
    };
  },
  components: {
    animatedInput: AnimatedInput
  },
  props: ["header"],
  methods: {}
};
</script>