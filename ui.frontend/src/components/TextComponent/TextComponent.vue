<template>
  <p>{{ newtext }}</p>
</template>

<script>
export default {
  name: 'TextComponent',
  props: {
    newtext: {
      type: String,
      default: 'Texto'
    }
  }
}
</script>

<style>
</style>
