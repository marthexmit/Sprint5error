<template>
    <TextComponent :newtext="Ftext" />
</template>

<script>
import TextComponent from '../TextComponent/TextComponent.vue'
export default {
  components: { TextComponent },
  name: 'FooterComponent',
  props: {
    Ftext: {
      type: String,
      default: 'created by Matheus Grigoleto - devChallenges.io'
    }
  }
}
</script>

<style>
</style>
