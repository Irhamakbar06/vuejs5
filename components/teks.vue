<script setup>
import { ref } from 'vue'

const teks = ref("")

</script>

<template>
  <input v-model="teks" placeholder="Type here">
  <p>{{ teks }}</p>
</template>