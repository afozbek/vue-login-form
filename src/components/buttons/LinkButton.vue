<template>
  <a class="a-linkButton">
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

<style lang="scss" scoped>
@import "@/scss/components/buttons/_linkButton.scss";

</style>
