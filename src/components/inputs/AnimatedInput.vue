<template>
  <div class="a-textInput">
    <input
      class="a-textInput__element"
      :class="{ '-animate': animateBorder }"
      placeholder=" "
      name="email"
      :type="inputType"
    />

    <div class="a-textInput__placeholder">{{ placeholder }}</div>

    <span class="a-textInput__pcAnimation" v-if="animateBorder"></span>
  </div>
</template>

<script>
export default {
  props: {
    inputType: {
      type: String,
      required: false,
      default: "text"
    },
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

<style lang="scss" scoped>
@import "@/scss/components/inputs/_animatedInput.scss";

</style>
