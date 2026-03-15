<template>
  <div class="destination-section bg-[#f8f5f0] p-6 lg:p-20 text-black py-16 flex flex-col md:flex-row gap-10 md:gap-20">
    
    <!-- DESKTOP VIEW: Kiri (Text dan List) -->
    <div class="hidden md:flex w-full md:w-[45%] flex-col pt-10 px-4 md:px-0">
      <h2 class="text-4xl md:text-5xl font-serif mb-6 leading-tight">Explore your next adventure with Pan Pacific</h2>
      <p class="text-sm md:text-base text-gray-600 mb-12 leading-relaxed max-w-md">
        Discover your next adventure with our handpicked travel inspiration, exciting guides, and spotlighted destinations from Pan Pacific that will ignite your wanderlust!
      </p>

      <div class="flex flex-col w-full max-w-sm mt-4">
        <div v-for="(dest, index) in destinations" :key="dest.name"
             class="py-6 border-b border-gray-300 flex justify-between items-center cursor-pointer px-6"
             :class="activeIndex === index ? 'bg-[#a38036] text-white border-none shadow-md' : 'text-black hover:bg-gray-100'"
             @click="activeIndex = index">
          <span class="font-serif text-2xl">{{ dest.name }}</span>
          <svg v-if="activeIndex === index" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="2" stroke="currentColor" class="w-5 h-5">
            <path stroke-linecap="round" stroke-linejoin="round" d="M13.5 4.5 21 12m0 0-7.5 7.5M21 12H3" />
          </svg>
        </div>
        <div class="py-6 border-b border-gray-300 flex justify-between items-center cursor-pointer hover:bg-gray-100 px-6">
           <span class="font-serif text-2xl text-gray-600">More destinations</span>
        </div>
      </div>
    </div>

    <!-- DESKTOP VIEW: Kanan (Gambar) -->
    <div class="hidden md:flex w-full md:w-[55%] justify-center md:justify-end">
      <div class="w-full md:w-[85%] h-[500px] md:h-[800px] overflow-hidden rounded-sm relative shadow-xl border-4 border-white">
         <img :src="destinations[activeIndex].image" :alt="destinations[activeIndex].name" class="w-full h-full object-cover" />
      </div>
    </div>

    <!-- MOBILE VIEW: Stacked Cards -->
    <div class="flex md:hidden flex-col w-full gap-4">
      <!-- Title on Mobile (Optional, depending if user wants it, but usually good to have. The mockup only shows cards, so we just show cards directly. If we need title, we can add it, but since user said "harusnya seperti yang saya berikan berikut", we'll just show the cards). Let's keep the layout simple matching the screenshot. -->
      <div v-for="dest in destinations" :key="'mob-' + dest.name" class="relative w-full h-40 overflow-hidden shadow-sm">
        <img :src="dest.image" :alt="dest.name" class="w-full h-full object-cover" />
        <div class="absolute inset-0 bg-black/30 flex items-center justify-center">
          <span class="text-white font-serif text-3xl font-normal tracking-wide drop-shadow-md">{{ dest.name }}</span>
        </div>
      </div>
      
      <div class="w-full mt-2">
        <button class="w-full bg-[#a88a42] text-white py-4 font-bold text-xs tracking-widest uppercase hover:bg-yellow-700">
          SHOW MORE
        </button>
      </div>
    </div>

  </div>
</template>

<script setup>
import { ref } from 'vue';

const destinations = ref([
  { name: 'Singapore', image: '/images/accordion2.png' },
  { name: 'Australia', image: '/images/melbourne.jpg' },
  { name: 'Malaysia', image: '/images/accordion3.png' },
  { name: 'China', image: '/images/lampion.jpg' },
  { name: 'Canada', image: '/images/snow.jpg' },
]);

const activeIndex = ref(1); // Default to Australia
</script>
