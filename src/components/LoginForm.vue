<template>
  <form class="m-loginForm">
    <h1 class="m-loginForm__desc">{{header}}</h1>

    <input class="m-loginForm__input" placeholder="Email" name="email" type="text" />

    <input class="m-loginForm__input" type="password" placeholder="Password" name="password" />

    <a class="m-loginForm__forgotBtn" href="#">Forgot Password?</a>

    <button type="submit" class="m-loginForm__submitBtn">Login</button>
  </form>
</template>

<script>
export default {
  props: ["header"]
};
</script>