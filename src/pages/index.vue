<template>
  <div ref="target">
    <RouterLink to="/">Home</RouterLink>
    <RouterLink to="/about">About</RouterLink>
    <div>{{ msg }}</div>
    <div class="text-3xl fond-bold underline">hello world from UnoCSS</div>
    <p>x: {{ x }}</p>
    <p>y: {{ y }}</p>
    <p>isOutside: {{ isOutside }}</p>
  </div>
</template>

<script setup lang="ts">
import { RouterLink } from 'vue-router/auto'
const msg = ref('Hello Vite + Vue 3 + TypeScript + UnoCSS!')
const target = ref(null)
const { x, y, isOutside } = useMouseInElement(target)
</script>

<style scoped></style>

<route lang="yaml">
meta:
  layout: default
</route>
