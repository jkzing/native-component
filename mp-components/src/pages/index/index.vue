<template>
  <div @click="handleClick">
    <card :text="motto"></card>
    <div>date: {{ date }}</div>
  </div>
</template>

<script>
import card from '@/components/card'

export default {
  mpType: 'component',
  properties: {
    date: String
  },

  data () {
    return {
      motto: 'Hello World from mpvue component'
    }
  },

  components: {
    card
  },

  methods: {
    handleClick () {
      console.log('click from mpvue component')
      this.$mp.page.triggerEvent('helloclick', { from: 'mpvue' }, {})
    }
  }
}
</script>

<style scoped>
</style>
