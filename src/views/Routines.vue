<template>
  <div class="text-white pt-4">
    <div class="space-y-3 px-8">
      <h1 class="text-4xl font-bold">Hi, Raul</h1>
      <p class="font-light">September 16, 2023</p>
    </div>

    <div class="px-8 mt-3 relative overflow-hidden">
      <transition-group name="slide" tag="div" class="flex">
        <div 
          v-for="(card, index) in cards" 
          :key="index" 
          class="w-[85vw] transform transition-transform"
          :class="{
            'scale-100': index === currentIndex,
            'scale-90': (index === currentIndex - 1 && currentIndex !== 0) || (index === currentIndex + 1 && currentIndex !== cards.length - 1),
            '-translate-x-full opacity-90': index < currentIndex,
            'translate-x-full opacity-90': index > currentIndex
          }"
        >
          <!-- Fake image -->
          <img :src="card.image" alt="" class="w-full h-[calc(100vh-30vh)] object-cover rounded-3xl">
          <div class="absolute bottom-8 left-10 space-y-1">
            <h2 class="text-4xl font-bold">{{ card.title }}</h2>
            <p class="tracking-wide">{{ card.description }}</p>
          </div>
        </div>
      </transition-group>
    </div>
  </div>
</template>

<script setup>
import { ref } from 'vue';
import firstCard from '../assets/img/stretching.jpg';
import secondCard from '../assets/img/lunge-stretch.jpg';
import thirdCard from '../assets/img/foot-stretch.jpg';

const currentIndex = ref(0); 
const cards = ref([
  {
    image: thirdCard,
    title: 'Daily',
    description: 'Improve for the long term'
  },
  {
    image: secondCard,
    title: 'Daily',
    description: 'Improve for the long term'
  },
  {
    image: firstCard,
    title: 'Daily',
    description: 'Improve for the long term'
  },
]);

const moveRight = () => {
  if (currentIndex.value < cards.value.length - 1) {
    currentIndex.value++;
  }
}

const moveLeft = () => {
  if (currentIndex.value > 0) {
    currentIndex.value--;
  }
}
</script>

<style>
.slide-enter-active, .slide-leave-active {
  transition: transform 1s;
}
.slide-enter, .slide-leave-to /* .slide-leave-active in <2.6 */ {
  transform: translateX(70vw);  /* You can adjust this value as needed */
}
</style>
