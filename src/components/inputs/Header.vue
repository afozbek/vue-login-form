<template>
  <h1 class="a-header">
    {{ title }}
  </h1>
</template>

<script>
export default {
  props: {
    title: {
      type: String,
      required: true
    }
  }
};
</script>

<style lang="scss" scoped>
@import "@/scss/components/inputs/_header.scss";

</style>
