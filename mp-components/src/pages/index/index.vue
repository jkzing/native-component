<template>
  <div>
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
      motto: 'Hello World from Native Component'
    }
  },

  components: {
    card
  },

  methods: {
  }
}
</script>

<style scoped>
</style>
