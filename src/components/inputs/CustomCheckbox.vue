<template>
  <div class="a-customCheckbox">
    <input
      class="a-customCheckbox__confirm"
      type="checkbox"
      :checked="checked"
      :name="name"
      :id="id"
    />

    <label
      class="a-customCheckbox__confirmLabel"
      :data-content="checkbox"
      :for="id"
    >
      <span class="a-customCheckbox__labelText">
        {{ labelText }}
      </span>
    </label>
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
    },
    checked: {
      type: Boolean,
      required: false,
      default: false
    }
  }
};
</script>

<style lang="scss" scoped>
@import "@/scss/components/inputs/_customCheckbox.scss";

</style>
