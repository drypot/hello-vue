<template>
  <h1>Hello Vue.js</h1>
  <p>{{ message }}</p>
</template>

<script setup>
import { defineProps, reactive } from 'vue'

defineProps({
  message: String
})
</script>

