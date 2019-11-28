<template>
  <div class="m-loginForm__inputGroup">
    <input
      class="m-loginForm__input"
      :class="{ '-animate': animateBorder }"
      placeholder=" "
      name="email"
      type="text"
    />

    <div class="m-loginForm__placeholder">{{ placeholder }}</div>

    <span class="m-loginForm__pcAnimation" v-if="animateBorder"></span>
  </div>
</template>

<script>
export default {
  props: {
    placeholder: {
      type: String,
      required: true
    },
    animateBorder: {
      type: Boolean,
      required: false,
      default: false
    }
  }
};
</script>
