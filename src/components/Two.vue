<template>
  <four-tag  @emit-four="GetNameFromFour"></four-tag>

</template>
  
  <script>
  import Four from './Four.vue'
  import Five from './Five.vue'
  import Six from './Six.vue'
  export default {
    data() {
        return {        
          name:''
        }
    },
    
    components: {
        'four-tag':Four
    },
    methods: {
        GetNameFromFour(xyz) {
          console.log(xyz)
            this.name=xyz
            this.$emit("emit-two",this.name)

        },
        
    }
  }
  </script>
  
  <style>
  
  </style>
  