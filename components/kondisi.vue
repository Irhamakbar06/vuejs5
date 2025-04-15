<script setup>
import {ref} from 'vue'

const mantap = ref(true)

function toggle(){
    mantap.value = !mantap.value;
}
</script>

<template>
    <button @click="toggle">toggle</button>
    <h1 v-if="mantap">benar sekali</h1>
    <h1 v-else>walaweee</h1>
    <h1>{{ mantap }}</h1>
</template>