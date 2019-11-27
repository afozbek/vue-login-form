<template>
  <div class="m-loginForm__checkboxWrapper">
    <input class="m-loginForm__confirm" type="checkbox" :name="name" :id="id" />

    <label class="m-loginForm__confirmLabel" :data-content="checkbox" :for="id">{{labelText}}</label>
  </div>
</template>

<script>
export default {
  props: {
    name: {
      type: String,
      required: true
    },
    id: {
      type: String,
      required: true
    },
    labelText: {
      type: String,
      required: true
    },
    checkbox: {
      type: String,
      required: false
      // \2713
      // \f00c
    }
  }
};
</script>