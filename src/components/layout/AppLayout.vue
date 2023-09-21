<!-- src/components/layout/AppLayout.vue -->
<template>
  <div class="wrapper min-h-screen bg-gradient-to-t from-slate-950 to-slate-900 flex flex-col">
    <Header class="flex-shrink-0 sticky top-0 z-10 bg-slate-900" />

    <div class="content-wrapper flex flex-row flex-grow overflow-y-auto pb-24">
      <!-- <Sidebar v-if="showSidebar" class="w-1/4 h-full overflow-y-auto" /> -->
      <main class="main-content flex-grow">
        <slot></slot>
      </main>
    </div>
    <Footer :currentView="currentView" class="flex-shrink-0 bg-slate-950"/>
  </div>
</template>

<script setup>
import Header from './Header.vue';
// import Sidebar from './Sidebar.vue'
import Footer from './Footer.vue';

import { ref, watch } from 'vue';
import { useRoute } from 'vue-router';

const route = useRoute();
const currentView = ref(route.name);

watch(
  () => route.name,
  (name) => {
    currentView.value = name;
  }
);
</script>

<style scoped>
.wrapper {
  position: relative;  /* This can stay to ensure any other positioned elements within .wrapper behave as expected */
}
</style>
