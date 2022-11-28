<script lang="ts" setup>
import { reactive, ref } from 'vue'

// step2
const counter = reactive({
  count: 0
})

console.log(counter.count) // 0
counter.count++

// step2
const message = ref('Hello World!')

console.log(message.value) // "Hello World!"
message.value = 'Changed'
</script>

<template>
  <h1>{{ message }}</h1>
  <p>count is: {{ counter.count }}</p>
  <h2>{{ message.split('').reverse().join('') }}</h2>
</template>