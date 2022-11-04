<template lang="">
  <div class="app-input">
    <label :for="id">{{ label }}</label>
    <input
      :type="type"
      :name="name"
      :placeholder="placeholder"
      :value="value"
      :class="['app-input__input']"
    />
    <span v-if="Boolean(errorMessage)" class="invalid-feedback">{{ errorMessage }}</span>
  </div>
</template>
<script>
export default {
  name: 'app-input',
  props: {
    value: { value: 'app-input' },
    errorMessage: { type: String, default: '' },
    label: { type: String, default: '' },
    name: { type: String },
    id: { type: String },
    type: { type: String, default: 'text' },
    placeholder: { type: String, default: '' },
  },
};
</script>
<style scoped lang="scss">
.app-input {
  display: flex;
  flex-direction: column;
  padding: 0 .8rem;
  label {
    margin-bottom: 8px;
    font-size: 1.3rem;

  }
  &__input {
    padding: 15px 4px 15px 20px;
    font-size: 1rem;
    border-radius: 0.25rem;
    border: 1px solid #000;
  }
}
</style>
