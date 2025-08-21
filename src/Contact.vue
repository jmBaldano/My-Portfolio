<!-- <script setup>

// import { Head } from '@inertiajs/vue3'
// const pageTitle = 'Profile'
</script>
<template>
<Head title =" | Contact" /> 
    <div class="Contact">
  <div class="sections">
      <h1 class="title py-16 mb-6 text-3xl font-bold text-center text-white">
        MY INFORMATION
      </h1>
<p>John Mark Baldano</p>

  
  <div class="flex items-center space-x-2 text-4xl text-white">
    
    <svg xmlns="http://www.w3.org/2000/svg" 
         fill="none" viewBox="0 0 24 24" 
         stroke-width="2" stroke="currentColor" 
         class="w-6 h-6">
      <path stroke-linecap="round" stroke-linejoin="round" 
            d="M12 21c4.418-4.418 8-7.582 8-11a8 8 0 10-16 0c0 3.418 3.582 6.582 8 11z" />
      <circle cx="12" cy="10" r="3" />
    </svg>
    <span>Quezon City, Philippines</span>
  </div>

  
  <div class="flex items-center space-x-2 text-white text-3xl">
    
    <svg xmlns="http://www.w3.org/2000/svg" 
         fill="none" viewBox="0 0 24 24" 
         stroke-width="2" stroke="currentColor" 
         class="w-6 h-6">
      <path stroke-linecap="round" stroke-linejoin="round" 
            d="M2 5a2 2 0 012-2h2.586a1 1 0 01.707.293l2.414 2.414a1 1 0 010 1.414L8.414 9.414c.379.379.861.879 1.293 1.293a15.978 15.978 0 005.586 3.586c.414.432.914.914 1.293 1.293l2.293-2.293a1 1 0 011.414 0l2.414 2.414a1 1 0 01.293.707V20a2 2 0 01-2 2h-1C9.82 22 2 14.18 2 5V5z" />
    </svg>
    <span>63-993-789-8675</span>
  </div>

  </div>
    </div>
    
</template> -->

<template>
<div  class="flex justify-center items-center min-h-screen bg-gray-900">
   
    <img
      src="https://picsum.photos/id/1018/600/400"
      alt="Preview"
      class="rounded-lg shadow-lg cursor-pointer hover:scale-105 transition"
      @click="open = true"
    />

   
    <div v-if="open" class="fixed inset-0 bg-black/70 flex justify-center items-center z-50">
      <div ref="container" class="relative w-[90%] max-w-xl aspect-video bg-white rounded-lg shadow-lg overflow-hidden">
        
        <div ref="carousel" class="flex transition-transform duration-500">
          <img src="https://picsum.photos/id/1018/800/600" class="w-full flex-shrink-0" alt="Slide 1" />
          <img src="https://picsum.photos/id/1015/800/600" class="w-full flex-shrink-0" alt="Slide 2" />
          <img src="https://picsum.photos/id/1019/800/600" class="w-full flex-shrink-0" alt="Slide 3" />
        </div>

        
        <button @click="prevSlide" class="absolute top-1/2 left-2 -translate-y-1/2 bg-black/50 text-white p-2 rounded-full">❮</button>
        <button @click="nextSlide" class="absolute top-1/2 right-2 -translate-y-1/2 bg-black/50 text-white p-2 rounded-full">❯</button>

        
        <button @click="open = false" class="absolute top-2 right-2 bg-red-500 text-white px-2 py-1 rounded">X</button>
      </div>
    </div>
  </div>
</template>

<script setup>
import { ref, onMounted, onBeforeUnmount } from "vue";

const open = ref(false);
const carousel = ref(null);
const container = ref(null);
const index = ref(0);

const totalSlides = 3;

function slideWidth() {
  return container.value ? container.value.clientWidth : 0;
}

function showSlide() {
  if (carousel.value) {
    carousel.value.style.transform = `translateX(-${index.value * slideWidth()}px)`;
  }
}

function nextSlide() {
  index.value = (index.value + 1) % totalSlides;
  showSlide();
}

function prevSlide() {
  index.value = (index.value - 1 + totalSlides) % totalSlides;
  showSlide();
}

// Make sure it resizes correctly when the window size changes
// function handleResize() {
//   showSlide();
// }

// onMounted(() => {
//   window.addEventListener("resize", handleResize);
// });

// onBeforeUnmount(() => {
//   window.removeEventListener("resize", handleResize);
// });
</script>


