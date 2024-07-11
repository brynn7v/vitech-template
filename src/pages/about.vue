<template>
  <div class="about">
    <RouterLink to="/">home</RouterLink>
    <RouterLink to="/about">about</RouterLink>
    <h1>This is an about page</h1>
  </div>
</template>

<script setup lang="ts"></script>

<style scoped></style>
<route lang="yaml">
meta:
  layout: home
</route>
