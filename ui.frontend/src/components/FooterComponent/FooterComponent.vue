<template>
  <footer>
    <TextComponent id="fStyled" :newtext="Ftext" :fontFamilyText="FfontText" :colorFieldText="FcolorText"/>
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
    },
    FfontText: {
      type: String,
      default: 'Montserrat'
    },
    FcolorText: {
      type: String,
      default: '#BDBDBD'
    }
  }
}
</script>

<style lang="scss">
@import url('https://fonts.googleapis.com/css2?family=Montserrat&display=swap');
@import './FooterComponent.scss'
</style>
