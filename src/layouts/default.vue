import router from '../router/index';
<template>
  <div class="flex">
    <router-link to="/">home</router-link>
    <router-link to="/about">about</router-link>
  </div>
  <router-view />
</template>

<script setup lang="ts"></script>

<style scoped></style>
