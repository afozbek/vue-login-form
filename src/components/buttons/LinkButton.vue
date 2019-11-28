<template>
  <a class="m-loginForm__forgotBtn">
    <!-- We can add fonts, texts etc -->
    <slot></slot>
  </a>
</template>

<script>
export default {
  props: {
    linkText: {
      type: String,
      required: true
    }
  }
};
</script>

<style></style>
