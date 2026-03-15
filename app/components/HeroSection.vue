<template>

<!-- COMPONENT: HeroSection.vue                 -->
    <div @click="nextSlide" class="hero-section relative w-full h-[600px] md:h-[800px] overflow-hidden bg-black cursor-pointer group">
      <!-- Carousel Container -->
      <div 
        class="flex w-full h-full transition-transform duration-700 ease-in-out" 
        :style="{ transform: `translateX(-${currentSlide * 100}%)` }"
      >
        <!-- Slides -->
        <div 
          v-for="(slide, index) in slides" 
          :key="index" 
          class="w-full h-full flex-shrink-0 relative"
        >
          <div 
            class="absolute inset-0 bg-cover bg-center"
            :style="{ backgroundImage: `url('${slide.image}')` }"
          ></div>
          <!-- Gradient Overlay Hitam Bawah (per slide to ensure text readability) -->
          <div class="absolute inset-0 bg-gradient-to-t from-black/80 via-black/30 to-transparent pointer-events-none"></div>

          <!-- Teks Diatas Gambar Kiri Bawah -->
          <div class="absolute bottom-16 md:bottom-24 left-6 md:left-24 text-white w-full pr-10 md:pr-24 z-10 pointer-events-none flex flex-col items-start">
            
            <p class="text-[10px] md:text-sm tracking-widest uppercase text-white mb-3 md:mb-5 font-bold flex items-center gap-1">
                 <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="2" stroke="currentColor" class="w-4 h-4 md:w-5 md:h-5">
                  <path stroke-linecap="round" stroke-linejoin="round" d="M15 10.5a3 3 0 1 1-6 0 3 3 0 0 1 6 0Z" />
                  <path stroke-linecap="round" stroke-linejoin="round" d="M19.5 10.5c0 7.142-7.5 11.25-7.5 11.25S4.5 17.642 4.5 10.5a7.5 7.5 0 1 1 15 0Z" />
                </svg>
                {{ slide.location }}
            </p>

            <!-- Judul Dinamis -->
            <h1 class="font-serif text-5xl md:text-7xl lg:text-8xl leading-tight text-white mb-6 md:mb-8 text-shadow-md max-w-5xl" v-html="slide.title"></h1>
            
            <!-- Capsule Categories -->
            <div class="flex gap-2 mx-1 flex-wrap mb-4 pointer-events-auto">
              <span v-for="tag in slide.tags" :key="tag" class="border border-white text-white bg-transparent text-[9px] md:text-[11px] py-1.5 md:py-2 px-3 md:px-5 rounded-full uppercase tracking-widest font-semibold hover:bg-white hover:text-black transition-colors cursor-pointer">
                {{ tag }}
              </span>
            </div>

            <div class="flex w-full mt-2 pointer-events-auto">
               <!-- Link More Details -->
               <a href="#" @click.stop class="text-xs md:text-sm font-sans text-white hover:text-gray-300 drop-shadow-md tracking-widest">
                 More details &rarr;
               </a>
            </div>
          </div>
        </div>
      </div>

      <!-- Dot Indicators dikanan bawah -->
      <div class="absolute bottom-16 md:bottom-24 right-6 md:right-24 flex gap-2 z-10 pointer-events-auto">
        <button 
          v-for="(slide, index) in slides" 
          :key="index"
          @click.stop="changeSlide(index)"
          class="w-1.5 h-1.5 md:w-2 md:h-2 rounded-full shadow-sm transition-colors duration-300"
          :class="currentSlide === index ? 'bg-[#b89441]' : 'bg-white opacity-60 hover:opacity-100'"
        ></button>
      </div>
    </div>
    <!-- END COMPONENT -->
</template>

<script setup>
import { ref } from 'vue';

const slides = ref([
  {
    image: '/images/melbourne.jpg',
    location: 'AUSTRALIA',
    title: 'The Essential Travel<br/>Guide To Melbourne',
    tags: ['SOLO TRAVELLER', 'FIRST-TIMER', 'LIFESTYLE', 'ROAD TRIP']
  },
  {
    image: '/images/snow.jpg',
    location: 'CANADA',
    title: 'Top Whistler honeymoon or <br/> babymoon staycation ideas',
    tags: ['COUPLE', 'WINTER', 'NATURE']
  }
]);

const currentSlide = ref(0);

const changeSlide = (index) => {
  currentSlide.value = index;
};

const nextSlide = () => {
  currentSlide.value = (currentSlide.value + 1) % slides.value.length;
};
</script>

<style scoped>
.text-shadow-md {
  text-shadow: 2px 2px 4px rgba(0,0,0,0.5);
}
</style>