<template>
  <div class="bottom-accordion bagian-explore p-0 text-white bg-[#1a1a1a]">
    <!-- Tab Headers (Desktop: flex-row, larger height requested by user) -->
    <div class="flex flex-col md:flex-row w-full h-32 md:h-28 lg:h-36 border-b border-gray-700">
      <div v-for="(kategori, index) in listKategori" :key="index"
           class="flex-1 relative cursor-pointer group h-full overflow-hidden"
           @click="activeIndex = index">
        <div class="absolute inset-0 bg-cover bg-center" :style="{ backgroundImage: `url('${kategori.gambar}')` }"></div>
        <div class="absolute inset-0" :class="activeIndex === index ? 'bg-black/20' : 'bg-black/70 group-hover:bg-black/40'"></div>
        <div class="relative z-10 w-full h-full flex items-center px-8">
          <span class="font-serif text-2xl lg:text-3xl text-white">{{ kategori.nama }}</span>
        </div>
      </div>
    </div>

    <!-- Active Tab Content Area - ONLY For Couples implemented as requested -->
    <div v-if="activeIndex === 0" class="w-full relative min-h-[600px] flex flex-col items-center pt-24 pb-0 px-6 md:px-12 lg:px-20 overflow-hidden">
      <!-- Background Image for Top Content -->
      <div class="absolute inset-0 bg-cover bg-center opacity-40 mix-blend-overlay h-[60%] lg:h-[70%]" style="background-image: url('/images/accordion1.png');"></div>
      <div class="absolute inset-0 bg-gradient-to-b from-[#1a1a1a]/90 via-[#1a1a1a]/60 to-[#1a1a1a] h-[60%] lg:h-[70%]"></div>

      <!-- Header Text & Button -->
      <div class="relative z-10 w-full max-w-7xl flex flex-col md:flex-row justify-between items-start gap-8 mb-16 lg:mb-24 px-4">
         <div class="w-full md:w-1/2">
           <h2 class="text-5xl md:text-7xl font-serif leading-tight">Memories Accross<br/>Generations</h2>
         </div>
         <div class="w-full md:w-2/5 flex flex-col items-start md:pt-4">
           <p class="text-gray-200 mb-8 leading-relaxed text-sm lg:text-base font-light">
             Explore destination, activities, and eitineraries that create lasting memories accross generations.
           </p>
           <button class="bg-[#a38036] text-white hover:bg-yellow-700 px-8 py-4 text-[10px] tracking-widest uppercase font-bold">
             DISCOVER MORE
           </button>
         </div>
      </div>

      <!-- Horizontal Cards Row (Dark Solid Background) -->
      <div class="w-screen bg-[#332e2e] py-16 px-6 md:px-12 lg:px-20 relative z-20 mt-auto flex justify-center border-t border-gray-700">
        <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8 w-full max-w-7xl">
           <!-- Cards -->
           <div v-for="i in 3" :key="i" class="flex flex-col gap-0">
              <p class="text-[9px] tracking-widest uppercase text-[#a38036] mb-3 font-bold flex items-center gap-1">
                 <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="2" stroke="currentColor" class="w-4 h-4"><path stroke-linecap="round" stroke-linejoin="round" d="M15 10.5a3 3 0 1 1-6 0 3 3 0 0 1 6 0Z" /><path stroke-linecap="round" stroke-linejoin="round" d="M19.5 10.5c0 7.142-7.5 11.25-7.5 11.25S4.5 17.642 4.5 10.5a7.5 7.5 0 1 1 15 0Z" /></svg>
                 CANADA
              </p>
              <img src="/images/snow.jpg" class="w-full h-48 sm:h-56 lg:h-64 object-cover shrink-0 mb-5" v-if="i===1 || i===3"/>
              <img src="/images/snow.jpg" class="w-full h-48 sm:h-56 lg:h-64 object-cover shrink-0 mb-5" v-if="i===2"/>
              <div class="flex flex-col justify-start">
                 <h3 class="font-serif text-xl lg:text-2xl leading-snug mb-5">Top Whistler honeymoon or babymoon staycation ideas</h3>
                 <div class="flex gap-2 flex-wrap">
                    <span class="border border-[#e5dfd3] text-[#e5dfd3] text-[9px] py-1.5 px-3 rounded-full uppercase tracking-widest bg-transparent">COUPLE</span>
                    <span class="border border-[#e5dfd3] text-[#e5dfd3] text-[9px] py-1.5 px-3 rounded-full uppercase tracking-widest bg-transparent">TRAVEL GUIDES</span>
                    <span class="border border-[#e5dfd3] text-[#e5dfd3] text-[9px] py-1.5 px-3 rounded-full uppercase tracking-widest bg-transparent mt-1">WINTER</span>
                    <span class="border border-[#e5dfd3] text-[#e5dfd3] text-[9px] py-1.5 px-3 rounded-full uppercase tracking-widest bg-transparent mt-1">HONEY MOON</span>
                    <span class="border border-[#e5dfd3] text-[#e5dfd3] text-[9px] py-1.5 px-3 rounded-full uppercase tracking-widest bg-transparent mt-1">NATURE</span>
                 </div>
              </div>
           </div>
        </div>
      </div>

    </div>
    
  </div>
</template>

<script setup>
import { ref } from 'vue';

const listKategori = ref([
  { nama: 'For Couples', gambar: '/images/accordion1.png' },
  { nama: 'For Family', gambar: '/images/accordion2.png' },
  { nama: 'For Business', gambar: '/images/accordion3.png' }
]);

const activeIndex = ref(0);
</script>
