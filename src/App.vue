<template>
  <div>
      <two-tag @emit-two="GetNameFromTwo"></two-tag>
      <Three-tag :sendToThree="gettwoname"></Three-tag>
  </div>

  
</template>

<script>

import Two from './components/Two.vue'
import Three from './components/Three.vue'

export default {
  data() {
    return {
       gettwoname:''
    }
  },
  components:{

    'two-tag':Two,
    'Three-tag':Three

  },
  methods: {
    GetNameFromTwo(xy) {
      console.log("======",xy)
     this.gettwoname = xy
    },

  }
}
</script>

<style>

</style>
