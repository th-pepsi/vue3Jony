<script setup lang="ts">
import {ref} from 'vue'
defineProps<{ msg: string }>()
const count = ref(1)
function setValue() {
  count.value++
}
</script>

<template>
  <div>
    <h1>{{ msg }}</h1>
    <div>{{ count }}</div>
    <button class="absolute bottom-5 right-0 left-0 text-center op30 fw300" @click="setValue">增加</button>
  </div>
</template>

<style scoped>
a {
  color: #42b983;
}

label {
  margin: 0 0.5em;
  font-weight: bold;
}

code {
  background-color: #eee;
  padding: 2px 4px;
  border-radius: 4px;
  color: #304455;
}
</style>
