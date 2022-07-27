<template>
  <img id="iStyled" :src="src" />
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

<style lang="scss" scoped>
@import './ImgComponent.scss'
</style>
