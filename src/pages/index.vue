<template>
  <div ref="target">
    <RouterLink to="/">Home</RouterLink>
    <RouterLink to="/about">About</RouterLink>
    <div>{{ msg }}</div>
    <div class="text-3xl fond-bold underline">hello world from UnoCSS</div>
    <p>x: {{ x }}</p>
    <p>y: {{ y }}</p>
    <p>isOutside: {{ isOutside }}</p>
    <HelloWorld />
    <UserUserComponent />
    <el-row class="mb-4">
      <el-button>Default</el-button>
      <el-button type="primary">Primary</el-button>
      <el-button type="success">Success</el-button>
      <el-button type="info">Info</el-button>
      <el-button type="warning">Warning</el-button>
      <el-button type="danger">Danger</el-button>
    </el-row>
    <div class="i-ph-anchor-simple-thin"></div>
    <div class="i-mdi-alarm text-orange-400"></div>
    <div class="i-logos-vue text-3xl"></div>
    <button class="i-carbon-sun dark:i-carbon-moon"></button>
    <div class="i-ion:airplane" style="color: red; font-size: 1.5rem"></div>
  </div>
</template>

<script setup lang="ts">
import { RouterLink } from 'vue-router/auto'
const msg = ref('Hello Vite + Vue 3 + TypeScript + UnoCSS!')
const target = ref(null)
const { x, y, isOutside } = useMouseInElement(target)
</script>

<style scoped></style>
