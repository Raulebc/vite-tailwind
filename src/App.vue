<script setup>
// import { ref, onMounted } from 'vue';

// const isDarkMode = ref(localStorage.getItem('darkMode') === 'true');

// const toggleDarkMode = () => {
//   isDarkMode.value = !isDarkMode.value;
//   localStorage.setItem('darkMode', isDarkMode.value);
// };

// onMounted(() => {
//   isDarkMode.value = localStorage.getItem('darkMode') === 'true';
// });

import AppLayout from './components/layout/AppLayout.vue';
</script>

<template>
  <AppLayout>
    <router-view></router-view>
  </AppLayout>
</template>

<style scoped>
</style>
