<template>
  <label :for="label">{{ label }}</label>
  <input type="text" :id="label" :placeholder="placeholder">
</template>

<script>
export default {
  name: 'TextInput',

  props: {
    label: String,
    placeholder: String
  }
}
</script>

<style scoped>
label {
  @apply block mt-3 mb-2;
}

input {
  @apply py-3 px-2 mb-10 border-2 border-gray-100 rounded w-full max-w-md;
}
</style>