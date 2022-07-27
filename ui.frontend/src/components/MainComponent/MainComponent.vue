<template>
    <div>
        <section id="sStyleMain">
            <Title id="mStyleTitle" :type="Mtype" :tMessage="Mtitle"/>
            <TextComponent id="mStyleText" :newtext="Mtext"/>
        </section>
    </div>
</template>

<script>

import TextComponent from '../TextComponent/TextComponent.vue'
import Title from '../Title/Title.vue'
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
    }
  },

  components: { TextComponent, Title }

}
</script>

<style lang="scss" scoped>
@import '../MainComponent/MainComponent.scss'
</style>
