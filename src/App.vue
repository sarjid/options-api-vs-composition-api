<template >
  <div>
  

    <button @click="increment">Count {{ counter }}</button>
  </div>
</template>


<script setup>
import {reactive, ref} from 'vue';
// export default {
  // data() {
  //   return {
  //     counter: 0
  //   }
  // },

  // methods: {
  //   increment(){
  //     this.counter += 1;
  //   }
  // },

  // setup() {
    const counter = ref(0);
    const test = reactive(0);

    const increment = () =>{
      counter.value += 1;
    };
    

  

    // return {counter,increment}


    
  // }
// }
</script>
<style lang="">
  
</style>