<template >
  <div>
    <input type="text" placeholder="your name" v-model="name">
    <h3>your name is: {{ name }}</h3>
  </div>
</template>


<script setup>
import {ref} from 'vue';
// export default {
  // data() {
  //   return {
  //     name: ''
  //   }
  // },

  // setup() {
    const name = ref("");


    
  // }
// }
</script>
<style lang="">
  
</style>