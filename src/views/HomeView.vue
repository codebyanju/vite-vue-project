<script setup>
import axios from 'axios'
import { onMounted } from 'vue'

onMounted(() => {
  const apiCall = axios.get('/hello/abc', { withCredentials: true }).then((response) => response)
  console.log('api', apiCall)
})
</script>

<template>
  <main>
    <h1>Hello Home View</h1>
  </main>
</template>
