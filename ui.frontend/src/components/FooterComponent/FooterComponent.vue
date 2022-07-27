<template>
  <footer>
    <TextComponent id="fStyled" :newtext="Ftext" />
  </footer>
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

<style lang="scss">
@import url('https://fonts.googleapis.com/css2?family=Montserrat&display=swap');
@import './FooterComponent.scss'
</style>
