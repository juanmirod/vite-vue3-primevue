<template>
  <h1>{{ msg }}</h1>

  <p>
    <a href="https://vitejs.dev/guide/features.html" target="_blank">Vite Documentation</a> |
    <a href="https://v3.vuejs.org/" target="_blank">Vue 3 Documentation</a> |
        <a href="https://www.primefaces.org/primevue" target="_blank">PrimeVue Documentation</a>
  </p>

  <p-button @click="state.count++" label="Count++"></p-button>
  <h2>{{ state.count }}</h2>

  <p>
    Edit
    <code>components/HelloWorld.vue</code> to test hot module replacement.
  </p>
</template>

<script setup>
import { defineProps, reactive } from 'vue';
import PButton from 'primevue/button';

defineProps({
  msg: String
})

const state = reactive({ count: 0 })
</script>

<style scoped>
a {
  color: #42b983;
}
</style>