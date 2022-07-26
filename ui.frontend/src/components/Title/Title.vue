<template>
    <div>
        <h1 v-if="type === 'h1'">{{ tMessage }}</h1>
        <h2 v-else-if="type === 'h2'">{{ tMessage }}</h2>
        <h3 v-else-if="type === 'h3'">{{ tMessage }}</h3>
        <h4 v-else-if="type === 'h4'">{{ tMessage }}</h4>
        <h5 v-else-if="type === 'h5'">{{ tMessage }}</h5>
        <h6 v-else-if="type === 'h6'">{{ tMessage }}</h6>
    </div>
</template>

<script>
export default {
  // eslint-disable-next-line
    name: "Title",
  props: {
    type: {
      type: String,
      default: 'h1'
    },
    tMessage: {
      type: String,
      default: 'testando'
    }
  }
}
</script>

<style>
</style>
