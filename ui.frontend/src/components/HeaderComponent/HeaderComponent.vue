<template>
    <div>
        <header>
            <Title :type="Htype" :tMessage="Htext" />
        </header>
    </div>
</template>

<script>
import Title from '../Title/Title.vue'
export default {
  // eslint-disable-next-line
    name: 'HeaderComponent',
  props: {
    Htext: {
      type: String,
      default: '404 not found'
    },
    Htype: {
      type: String,
      default: 'h1'
    }
  },
  components: { Title }
}
</script>

<style>
</style>
