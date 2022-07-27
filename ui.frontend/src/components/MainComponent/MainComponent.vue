<template>
    <div>
        <main>
            <Title id="mStyleTitle" :type="Mtype" :tMessage="Mtitle" />
            <TextComponent id="mStyleText" :newtext="Mtext" />
            <Button id="bStyled" :Btext="Mbtext" />
        </main>
    </div>
</template>

<script>

import TextComponent from '../TextComponent/TextComponent.vue'
import Title from '../Title/Title.vue'
import Button from '../Button/Button.vue'
export default {
  name: 'MainComponent',
  props: {
    Mtype: {
      type: String,
      default: 'h1'
    },
    Mtitle: {
      type: String,
      default: 'I have bad news for you'
    },
    Mtext: {
      type: String,
      default: 'The page you are looking for might be removed or is temporarily unavailable'
    },
    Mbtext: {
      type: String,
      default: 'BACK TO HOME PAGE'
    }
  },

  components: { TextComponent, Title, Button }

}
</script>

<style lang="scss" scoped>
@import url('https://fonts.googleapis.com/css2?family=Space+Mono&display=swap');
@import '../MainComponent/MainComponent.scss'
</style>
