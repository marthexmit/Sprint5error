<template>
  <img :src="src" />
</template>

<script>
export default {
  name: 'ImageComponent',
  props: {
    src: {
      type: String
    }
  }
}
</script>

<style>
</style>
