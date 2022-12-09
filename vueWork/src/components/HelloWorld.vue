<script setup>
import { ref, reactive } from 'vue'

// defineProps({
//   msg: String
// })

const state = reactive({ symbol: "" })


function addText(value) {
  let arr = value.split('').shift().toUpperCase();

  // state.symbol = value.split('')

  console.log(value, arr);
}



</script>
  
<template>
  <input v-model="text" placeholder="Text" @keypress.enter="addText(text)">
  <p>{{state.symbol}}</p>
</template>

<style scoped lang="sass">


</style>
