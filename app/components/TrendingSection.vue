<template>

<!-- COMPONENT: TrendingSection.vue              -->

    <div class="trending-section trending-gelap bg-[#232323] text-white pt-16 pb-12 px-6 md:px-20">
      <h2 class="text-4xl md:text-5xl font-serif text-center mb-4">What's trending</h2>
      <p class="text-center text-xs tracking-widest text-[#a8a8a8] mb-12 px-4 uppercase">Our top picks guaranteed to scratch that travel itch.</p>

      <!-- Horizontal Carousel dari daisyUI -->
      <!-- Menggunakan space-x-0 karena gap diatur di dalam item, atau gunakan gap. Kita gunakan gap-6. -->
      <div class="carousel carousel-center rounded-none w-full gap-4 md:gap-6 pb-4">
        
        <!-- Di Desktop (lg), setiap item ambil 1/3 (33.333%) dikurangi sedikit untuk scrollbar/gap. -->
        <!-- Gunakan w-[85%] untuk mobile, mb-[45%] tablet, lg:w-[calc(33.333%-16px)] -->
        
        <!-- Slide 1 -->
        <div class="carousel-item w-[85%] md:w-[45%] lg:w-[calc(33.333%-1rem)] relative overflow-hidden group h-[450px] md:h-[550px] cursor-pointer">
          <img src="/images/balonudara.png" alt="Balon Udara" class="w-full h-full object-cover   " />
          <!-- Gradient di bawah murni untuk membuat tulisan putih terbaca, no overlay keseluruhan -->
          <div class="absolute inset-0 bg-gradient-to-t from-black/80 via-black/20 to-transparent pointer-events-none"></div>
          
          <div class="absolute bottom-0 left-0 w-full p-6 md:p-8 flex flex-col justify-end">
             <div class="flex gap-2 mb-3">
               <p class="text-[9px] uppercase tracking-widest font-bold flex items-center gap-1 text-white">
                 <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="2" stroke="currentColor" class="w-3 h-3 text-white">
                  <path stroke-linecap="round" stroke-linejoin="round" d="M15 10.5a3 3 0 1 1-6 0 3 3 0 0 1 6 0Z" />
                  <path stroke-linecap="round" stroke-linejoin="round" d="M19.5 10.5c0 7.142-7.5 11.25-7.5 11.25S4.5 17.642 4.5 10.5a7.5 7.5 0 1 1 15 0Z" />
                </svg>
                CANADA
               </p>
            </div>
            <h2 class="font-serif text-3xl md:text-4xl leading-snug mb-5 text-white text-shadow-sm">Top Whistler Honeymoon Or Babymoon Staycation Ideas</h2>
            <div class="flex gap-2 flex-wrap">
                <span class="border border-[#b89441] text-[#b89441] text-[9px] py-1 px-3 rounded-full uppercase tracking-widest bg-transparent">COUPLE</span>
                <span class="border border-[#b89441] text-[#b89441] text-[9px] py-1 px-3 rounded-full uppercase tracking-widest bg-transparent">TRAVEL GUIDES</span>
                <span class="border border-[#b89441] text-[#b89441] text-[9px] py-1 px-3 rounded-full uppercase tracking-widest bg-transparent">WINTER</span>
                <span class="border border-[#b89441] text-[#b89441] text-[9px] py-1 px-3 rounded-full uppercase tracking-widest bg-transparent mt-1">HONEY MOON</span>
                <span class="border border-[#b89441] text-[#b89441] text-[9px] py-1 px-3 rounded-full uppercase tracking-widest bg-transparent mt-1">NATURE</span>
            </div>
          </div>
        </div>

        <!-- Slide 2 -->
        <div class="carousel-item w-[85%] md:w-[45%] lg:w-[calc(33.333%-1rem)] relative overflow-hidden group h-[450px] md:h-[550px] cursor-pointer">
          <img src="/images/balonudara.png" alt="Balon Udara" class="w-full h-full object-cover   " />
          <div class="absolute inset-0 bg-gradient-to-t from-black/80 via-black/20 to-transparent pointer-events-none"></div>
          
          <div class="absolute bottom-0 left-0 w-full p-6 md:p-8 flex flex-col justify-end">
             <div class="flex gap-2 mb-3">
               <p class="text-[9px] uppercase tracking-widest font-bold flex items-center gap-1 text-white">
                 <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="2" stroke="currentColor" class="w-3 h-3 text-white">
                  <path stroke-linecap="round" stroke-linejoin="round" d="M15 10.5a3 3 0 1 1-6 0 3 3 0 0 1 6 0Z" />
                  <path stroke-linecap="round" stroke-linejoin="round" d="M19.5 10.5c0 7.142-7.5 11.25-7.5 11.25S4.5 17.642 4.5 10.5a7.5 7.5 0 1 1 15 0Z" />
                </svg>
                CANADA
               </p>
            </div>
            <h2 class="font-serif text-3xl md:text-4xl leading-snug mb-5 text-white text-shadow-sm">Top Whistler Honeymoon Or Babymoon Staycation Ideas</h2>
            <div class="flex gap-2 flex-wrap">
                <span class="border border-[#b89441] text-[#b89441] text-[9px] py-1 px-3 rounded-full uppercase tracking-widest bg-transparent">COUPLE</span>
                <span class="border border-[#b89441] text-[#b89441] text-[9px] py-1 px-3 rounded-full uppercase tracking-widest bg-transparent">TRAVEL GUIDES</span>
                <span class="border border-[#b89441] text-[#b89441] text-[9px] py-1 px-3 rounded-full uppercase tracking-widest bg-transparent">WINTER</span>
                <span class="border border-[#b89441] text-[#b89441] text-[9px] py-1 px-3 rounded-full uppercase tracking-widest bg-transparent mt-1">HONEY MOON</span>
                <span class="border border-[#b89441] text-[#b89441] text-[9px] py-1 px-3 rounded-full uppercase tracking-widest bg-transparent mt-1">NATURE</span>
            </div>
          </div>
        </div>

        <!-- Slide 3 -->
        <div class="carousel-item w-[85%] md:w-[45%] lg:w-[calc(33.333%-1rem)] relative overflow-hidden group h-[450px] md:h-[550px] cursor-pointer">
          <img src="/images/balonudara.png" alt="Balon Udara" class="w-full h-full object-cover   " />
          <div class="absolute inset-0 bg-gradient-to-t from-black/80 via-black/20 to-transparent pointer-events-none"></div>
          
          <div class="absolute bottom-0 left-0 w-full p-6 md:p-8 flex flex-col justify-end">
             <div class="flex gap-2 mb-3">
               <p class="text-[9px] uppercase tracking-widest font-bold flex items-center gap-1 text-white">
                 <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="2" stroke="currentColor" class="w-3 h-3 text-white">
                  <path stroke-linecap="round" stroke-linejoin="round" d="M15 10.5a3 3 0 1 1-6 0 3 3 0 0 1 6 0Z" />
                  <path stroke-linecap="round" stroke-linejoin="round" d="M19.5 10.5c0 7.142-7.5 11.25-7.5 11.25S4.5 17.642 4.5 10.5a7.5 7.5 0 1 1 15 0Z" />
                </svg>
                CANADA
               </p>
            </div>
            <h2 class="font-serif text-3xl md:text-4xl leading-snug mb-5 text-white text-shadow-sm">Top Whistler Honeymoon Or Babymoon Staycation Ideas</h2>
            <div class="flex gap-2 flex-wrap">
                <span class="border border-[#b89441] text-[#b89441] text-[9px] py-1 px-3 rounded-full uppercase tracking-widest bg-transparent">COUPLE</span>
                <span class="border border-[#b89441] text-[#b89441] text-[9px] py-1 px-3 rounded-full uppercase tracking-widest bg-transparent">TRAVEL GUIDES</span>
                <span class="border border-[#b89441] text-[#b89441] text-[9px] py-1 px-3 rounded-full uppercase tracking-widest bg-transparent">WINTER</span>
                <span class="border border-[#b89441] text-[#b89441] text-[9px] py-1 px-3 rounded-full uppercase tracking-widest bg-transparent mt-1">HONEY MOON</span>
                <span class="border border-[#b89441] text-[#b89441] text-[9px] py-1 px-3 rounded-full uppercase tracking-widest bg-transparent mt-1">NATURE</span>
            </div>
          </div>
        </div>

      </div>
    </div>
    <!-- END COMPONENT: Trending.vue -->
</template>

<style scoped>
/* Sembunyikan scrollbar untuk tampilan yg clean */
.carousel::-webkit-scrollbar {
  display: none;
}
.carousel {
  -ms-overflow-style: none;
  scrollbar-width: none;
}
.text-shadow-sm {
  text-shadow: 1px 1px 3px rgba(0,0,0,0.5);
}
</style>