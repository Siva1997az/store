<template>
  <eight-tag :sendToEight="sevenname"></eight-tag>
</template>

<script>

import Eight from './Eight.vue'
export default {
  data() {
      return {
          sevenname:''
      }
  },
  watch: {
      sendToSeven(val) {
        this.sevenname = val
      }
  },
  props: ['sendToSeven'],
  methods: {
     
    
     },
  
  components: {
      'eight-tag':Eight
  },
}
</script>

<style>

</style>
