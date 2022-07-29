<template>
  <main>
    <Title id="mStyleTitle" :type="Mtype" :tMessage="Mtitle" :fontFamily="MfontTitle" :colorField="McolorTitle"/>
    <TextComponent id="mStyleText" :newtext="Mtext" :fontFamilyText="MfontText" :colorFieldText="McolorText"/>
    <Button id="bStyled" :Btext="Mbtext" :fontFamilyButton="Mbfont" :backColorButton="MbBackcolor" :colorFieldButton="Mbcolor" :hoverButton="Mbhover" />
  </main>
</template>

<script>

import TextComponent from '../TextComponent/TextComponent.vue'
import Title from '../Title/Title.vue'
import Button from '../Button/Button.vue'
export default {
  // eslint-disable-next-line
  name: 'MainComponent',
  props: {
    Mtitle: {
      type: String,
      default: 'I have bad news for you'
    },
    Mtype: {
      type: String,
      default: 'h1'
    },
    Mtext: {
      type: String,
      default: 'The page you are looking for might be removed or is temporarily unavailable'
    },
    Mbtext: {
      type: String,
      default: 'BACK TO HOME PAGE'
    },
    MfontTitle: {
      type: String,
      default: 'Space Mono'
    },
    McolorTitle: {
      type: String,
      default: '#333333'
    },
    MfontText: {
      type: String,
      default: 'Space Mono'
    },
    McolorText: {
      type: String,
      default: '#4f4f4f'
    },
    Mbfont: {
      type: String,
      default: 'Space Mono'
    },
    MbBackcolor: {
      type: String
    },
    Mbcolor: {
      type: String,
      default: '#FFFFFF'
    }
  },

  components: { TextComponent, Title, Button }

}
</script>

<style lang="scss" scoped>
@import url('https://fonts.googleapis.com/css2?family=Space+Mono&display=swap');
@import '../MainComponent/MainComponent.scss'
</style>
