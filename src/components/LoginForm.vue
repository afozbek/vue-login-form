<template>
  <form class="m-loginForm">
    <Header :title="title" />

    <div class="m-loginForm__group">
      <animated-input placeholder="Email" animateBorder />
    </div>

    <div class="m-loginForm__group">
      <animated-input
        placeholder="Password"
        animateBorder
        inputType="password"
      />
    </div>

    <div class="m-loginForm__group -mg-lg">
      <div class="m-loginForm__rememberWrapper">
        <custom-checkbox
          name="remember_me"
          id="remember_me"
          labelText="Remember Me 😉"
          checkbox="✔︎"
        ></custom-checkbox>

        <link-button href="#" linkText="Forgot Password">
          I forgot password 🤦🏻‍♂️
        </link-button>
      </div>
    </div>

    <!-- <div class="a-showCase">
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
    </div> -->

    <submit-button>Login</submit-button>
  </form>
</template>

<script>
import Header from "./inputs/Header.vue";
import AnimatedInput from "./inputs/AnimatedInput.vue";
import CustomCheckbox from "./inputs/CustomCheckbox.vue";
import LinkButton from "./buttons/LinkButton.vue";
import SubmitButton from "./buttons/SubmitButton.vue";

export default {
  data() {
    return {
      email: "",
      password: "",
      rememberMe: false
    };
  },
  components: {
    Header,
    AnimatedInput,
    CustomCheckbox,
    LinkButton,
    SubmitButton
  },
  props: {
    title: String
  }
};
</script>

<style lang="scss" scoped>
@import "@/scss/components/forms/_loginForm.scss";

</style>
