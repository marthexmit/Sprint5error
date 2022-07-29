<template>
        <header>
            <Title id="hStyled" :type="Htype" :tMessage="Htext" :fontFamily="Hfont" :colorField="Hcolor" />
        </header>
</template>

<script>

import Title from '../Title/Title.vue'
export default {
  // eslint-disable-next-line
    name: 'HeaderComponent',
  props: {
    Htext: {
      type: String,
      default: '404 NOT FOUND'
    },
    Htype: {
      type: String,
      default: 'h1'
    },
    Hfont: {
      type: String,
      default: 'Inconsolata'
    },
    Hcolor: {
      type: String,
      default: '#333333'
    }
  },
  components: { Title }
}
</script>

<style lang="scss" scoped>
@import url('https://fonts.googleapis.com/css2?family=Inconsolata&display=swap');
@import './HeaderComponent.scss'
</style>
