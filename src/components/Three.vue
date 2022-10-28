<template>
  <seven-tag :sendToSeven="threename"></seven-tag>
</template>

<script>

import Seven from './Seven.vue'
export default {
  data() {
      return {
          threename:''
      }
  },
  props: ['sendToThree'],
  watch: {
    sendToThree(val) {
      console.log(val, "watch || Three.vue")
      this.threename=val
    }
  },
  methods: {
     
    
     },
   mounted () {
    console.log(this.sendToThree, "Three.vue")
   },
  components: {
      'seven-tag':Seven
  },
}
</script>

<style>

</style>
