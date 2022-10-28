<template>
    <h1 @click="SendToTwo">click</h1>
</template>
  
  <script>
  
  
  export default {

  data(){
    return{
        
    }
  },
  mounted() {
    this.$emit('emit-four','siva100')

  },
//   props: ['name'],
  methods: {
    SendToTwo() {
        this.$emit('emit-four','siva')
    }
  },
    
  }
  </script>
  
  <style>
  
  </style>
  