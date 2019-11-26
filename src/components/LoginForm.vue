<template>
  <form class="m-loginForm">
    <h1 class="m-loginForm__desc">{{ header }}</h1>

    <div class="m-loginForm__group">
      <div class="m-loginForm__inputGroup">
        <input class="m-loginForm__input" v-model="email" placeholder=" " name="email" type="text" />

        <div class="m-loginForm__placeholder">Email</div>

        <span class="m-loginForm__pcAnimation"></span>
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
        <span class="m-loginForm__pcAnimation"></span>
      </div>
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
export default {
  data() {
    return {
      email: "",
      password: "",
      rememberMe: false
    };
  },
  props: ["header"],
  methods: {}
};
</script>