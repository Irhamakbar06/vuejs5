<script setup>
import {ref} from 'vue'

const nama = ref('irham')
</script>

<template>
<h1 v-bind:class="nama">irham ganteng</h1>
</template>

<style scoped>
.irham{
    color: violet;
    font-size: 40px;
}
</style>