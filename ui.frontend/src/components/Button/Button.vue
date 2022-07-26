<template>
  <button>{{ Btext }}</button>
</template>

<script>
export default {
  name: 'ButtonComponent',
  props: {
    Btext: {
      type: String,
      default: 'BACK TO HOME PAGE'
    }
  }
}
</script>

<style>
</style>
