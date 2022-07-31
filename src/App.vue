<template>
  <div>
    {{ name1 }}
    {{ name2 }}
    {{ fullName }}

    <button @click="changeFunction">Change</button>
  </div>
</template>

<script setup>
import { ref, onMounted, computed } from "vue";
// export default {
//   data() {
//     return {
//       name1: "jishan",
//       name2: "Hasan",
//     };
//   },

//   methods: {
//     changeFunction() {
//       this.name1 = "Hasan";
//       this.name2 = "testing..";
//     },
//   },

//   // mounted() {
//   //   this.changeFunction();
//   // },

//   computed:{
//     fullName(){
//       return this.name1 + this.name2;
//     }
//   }
// };

const name1 = ref("Jishan");
const name2 = ref("Hasan");

const changeFunction = () => {
  name1.value = "Hasan";
  name2.value = "testing..";
};

// onMounted(() => {
//   changeFunction();
// })

const fullName = computed(() => {
  return name1.value + name2.value;
});
</script>

<style lang=""></style>
