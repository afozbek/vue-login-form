<template>
  <form class="m-loginForm">
    <h1 class="m-loginForm__desc">{{header}}</h1>
    <div class="m-loginForm__inputGroup">
      <input class="m-loginForm__input" v-model="email" placeholder=" " name="email" type="text" />
      <div class="m-loginForm__placeholder">Email</div>
    </div>

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

    <a class="m-loginForm__forgotBtn" href="#">Forgot Password?</a>

    <button type="submit" class="m-loginForm__submitBtn">Login</button>
  </form>
</template>

<script>
export default {
  data() {
    return {
      email: "",
      password: ""
    };
  },
  props: ["header"],
  methods: {}
};
</script>