<script setup>
import { ref, watch } from 'vue'

const username = ref('')
const warning = ref('')

watch(username, (val) => {
  if (val.length > 10) {
    warning.value = 'Username terlalu panjang'
  } else {
    warning.value = ''
  }
})
</script>

<template>
  <div>
    <label>Username:</label>
    <input v-model="username" type="text" placeholder="Masukkan username" />
    <p v-if="warning" style="color: red">{{ warning }}</p>
  </div>
</template>
