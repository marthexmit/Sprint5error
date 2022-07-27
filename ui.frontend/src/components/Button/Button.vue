<template>
  <button>{{ Btext }}</button>
</template>

<script>
export default {
  name: 'ButtonComponent',
  props: {
    Btext: {
      type: String
    }
  }
}
</script>

<style>
</style>
