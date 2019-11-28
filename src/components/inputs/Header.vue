<template>
  <h1 class="m-loginForm__desc">{{ title }}</h1>
</template>

<script>
export default {
  props: {
    title: String,
    required: true
  }
};
</script>
