<script setup>
 import {ref} from 'vue'

 const count = ref(5)
 const kata = ref('take a chance with me')
</script>

<template>
    <h1>{{ kata }}</h1>
    <p>{{ count }}</p>
</template>