<template>
  <form class="m-loginForm">
    <h1 class="m-loginForm__desc">{{ header }}</h1>

    <div class="m-loginForm__group">
      <div class="m-loginForm__inputGroup">
        <input class="m-loginForm__input" v-model="email" placeholder=" " name="email" type="text" />

        <div class="m-loginForm__placeholder">Email</div>
      </div>
    </div>

    <div class="m-loginForm__group">
      <div class="m-loginForm__inputGroup">
        <input
          class="m-loginForm__input"
          v-model="password"
          placeholder=" "
          type="password"
          name="password"
        />

        <div class="m-loginForm__placeholder">Password</div>
      </div>
    </div>

    <div class="m-loginForm__group -mg-lg">
      <div class="m-loginForm__rememberWrapper">
        <custom-checkbox name="remember_me" id="remember_me" labelText="Furkan" checkbox="✔︎"></custom-checkbox>

        <a class="m-loginForm__forgotBtn" href="#">Forgot Password?</a>
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