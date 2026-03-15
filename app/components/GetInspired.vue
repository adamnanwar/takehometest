<template>
  <div class="get-inspired globe-trot bg-[#24211f] text-white p-6 md:p-12 lg:px-20 pt-32 pb-20 flex flex-col items-center overflow-hidden">
    
    <!-- Container Utama: Stack pada Mobile, Side-by-Side pada Desktop -->
    <div class="w-full max-w-7xl flex flex-col lg:flex-row gap-10 lg:gap-16 items-start">
      
      <!-- Bagian Kiri (Desktop) / Atas (Mobile): Title, Menus, Arrows -->
      <div class="w-full lg:w-[30%] flex flex-col shrink-0 text-center lg:text-left">
        <!-- Title -->
        <h2 class="text-5xl md:text-7xl lg:text-5xl xl:text-6xl font-serif leading-tight mb-8">Globe-trot with<br/>Pan Pacific</h2>
        
        <!-- Horizontal Pills (Mobile) & Vertical List (Desktop) -->
        <div class="flex flex-row lg:flex-col overflow-x-auto lg:overflow-visible whitespace-nowrap gap-3 lg:gap-4 mb-10 w-full no-scrollbar items-center lg:items-start justify-start lg:justify-start px-2 lg:px-0">
          <button class="text-gray-300 hover:text-white bg-transparent border border-transparent hover:border-gray-500 rounded-full px-4 py-2 lg:px-0 lg:py-1 lg:rounded-none lg:border-none lg:text-left text-[10px] font-bold uppercase tracking-widest shrink-0 transition-all">ALL</button>
          <button class="text-gray-300 hover:text-white bg-transparent border border-transparent hover:border-gray-500 rounded-full px-4 py-2 lg:px-0 lg:py-1 lg:rounded-none lg:border-none lg:text-left text-[10px] font-bold uppercase tracking-widest shrink-0 transition-all">ROAD TRIPS</button>
          <button class="text-gray-300 hover:text-white bg-transparent border border-transparent hover:border-gray-500 rounded-full px-4 py-2 lg:px-0 lg:py-1 lg:rounded-none lg:border-none lg:text-left text-[10px] font-bold uppercase tracking-widest shrink-0 transition-all">SUSTAINABLE TRAVEL</button>
          <button class="bg-[#a88a42] text-white rounded-full px-6 py-2.5 text-[10px] font-bold tracking-widest uppercase shadow-md shrink-0 lg:w-auto text-left">PHOTO JOURNAL</button>
          <button class="text-gray-300 hover:text-white bg-transparent border border-transparent hover:border-gray-500 rounded-full px-4 py-2 lg:px-0 lg:py-1 lg:rounded-none lg:border-none lg:text-left text-[10px] font-bold uppercase tracking-widest shrink-0 transition-all">ROMANTIC</button>
          <button class="text-gray-300 hover:text-white bg-transparent border border-transparent hover:border-gray-500 rounded-full px-4 py-2 lg:px-0 lg:py-1 lg:rounded-none lg:border-none lg:text-left text-[10px] font-bold uppercase tracking-widest shrink-0 transition-all">FAMILY BONDING</button>
          <button class="text-gray-300 hover:text-white bg-transparent border border-transparent hover:border-gray-500 rounded-full px-4 py-2 lg:px-0 lg:py-1 lg:rounded-none lg:border-none lg:text-left text-[10px] font-bold uppercase tracking-widest shrink-0 transition-all">JET SETTING</button>
        </div>

        <!-- Arrow Controls (Desktop: ditaruh di kolom kiri bawah) -->
        <div class="hidden lg:flex gap-4 mt-8 items-center cursor-pointer justify-start">
          <div class="w-10 h-10 rounded-full border border-gray-600 flex items-center justify-center hover:bg-gray-800 transition-colors">
            <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="w-4 h-4 text-gray-400">
              <path stroke-linecap="round" stroke-linejoin="round" d="M15.75 19.5 8.25 12l7.5-7.5" />
            </svg>
          </div>
          <div class="w-10 h-10 rounded-full border border-gray-600 flex items-center justify-center hover:bg-gray-800 transition-colors">
            <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="w-4 h-4 text-gray-400">
              <path stroke-linecap="round" stroke-linejoin="round" d="m8.25 4.5 7.5 7.5-7.5 7.5" />
            </svg>
          </div>
        </div>
      </div>

      <!-- Bagian Kanan (Desktop) / Bawah (Mobile): Carousel / Cards Area -->
      <div class="w-full lg:w-[70%]">
        <div class="carousel carousel-center rounded-none w-full gap-6 pb-4 overflow-x-auto overflow-y-hidden snap-x snap-mandatory">
          <!-- Card 1 -->
          <div class="carousel-item w-[85%] sm:w-[55%] lg:w-[50%] flex-col bg-[#f8f5f0] shrink-0 h-[480px] snap-center lg:snap-start">
            <div class="h-[55%] w-full rounded-none">
              <img src="/images/snow.jpg" class="w-full h-full object-cover" />
            </div>
            <div class="p-8 text-black flex flex-col justify-start h-[45%] relative border-t-4 border-[#b89441]">
               <p class="text-[9px] text-[#b89441] tracking-widest mb-3 uppercase font-bold flex items-center gap-1">
                 <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="2" stroke="currentColor" class="w-3 h-3">
                   <path stroke-linecap="round" stroke-linejoin="round" d="M15 10.5a3 3 0 1 1-6 0 3 3 0 0 1 6 0Z" />
                   <path stroke-linecap="round" stroke-linejoin="round" d="M19.5 10.5c0 7.142-7.5 11.25-7.5 11.25S4.5 17.642 4.5 10.5a7.5 7.5 0 1 1 15 0Z" />
                 </svg>
                CANADA
              </p>
              <h2 class="font-serif text-2xl leading-snug mb-4">Top Whistler Honeymoon Staycation Ideas</h2>
              <div class="flex gap-2 flex-wrap mt-auto">
                <span class="border border-gray-400 text-gray-500 text-[8px] py-1.5 px-3 rounded-full uppercase tracking-widest">COUPLE</span>
                <span class="border border-gray-400 text-gray-500 text-[8px] py-1.5 px-3 rounded-full uppercase tracking-widest">WINTER</span>
              </div>
               <div class="absolute bottom-0 right-0 bg-[#b89441] w-12 h-12 flex items-center justify-center text-white cursor-pointer hover:bg-yellow-700 ">
                 <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="2" stroke="currentColor" class="w-5 h-5">
                   <path stroke-linecap="round" stroke-linejoin="round" d="M13.5 4.5 21 12m0 0-7.5 7.5M21 12H3" />
                 </svg>
              </div>
            </div>
          </div>
          
          <!-- Card 2 -->
          <div class="carousel-item w-[85%] sm:w-[55%] lg:w-[50%] flex-col bg-[#f8f5f0] shrink-0 h-[480px] snap-center lg:snap-start">
            <div class="h-[55%] w-full rounded-none">
              <img src="/images/barongsai.jpg" class="w-full h-full object-cover" />
            </div>
            <div class="p-8 text-black flex flex-col justify-start h-[45%] relative border-t-4 border-transparent hover:border-[#b89441] transition-all">
               <p class="text-[9px] text-[#b89441] tracking-widest mb-3 uppercase font-bold flex items-center gap-1">
                 <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="2" stroke="currentColor" class="w-3 h-3">
                   <path stroke-linecap="round" stroke-linejoin="round" d="M15 10.5a3 3 0 1 1-6 0 3 3 0 0 1 6 0Z" />
                   <path stroke-linecap="round" stroke-linejoin="round" d="M19.5 10.5c0 7.142-7.5 11.25-7.5 11.25S4.5 17.642 4.5 10.5a7.5 7.5 0 1 1 15 0Z" />
                 </svg>
                SINGAPORE
              </p>
              <h2 class="font-serif text-2xl leading-snug mb-4">Things to do on Chinese New Year</h2>
              <div class="flex gap-2 flex-wrap mt-auto">
                <span class="border border-gray-400 text-gray-500 text-[8px] py-1.5 px-3 rounded-full uppercase tracking-widest">LOCALS</span>
                <span class="border border-gray-400 text-gray-500 text-[8px] py-1.5 px-3 rounded-full uppercase tracking-widest">CULTURE</span>
              </div>
               <div class="absolute bottom-0 right-0 bg-[#b89441] w-12 h-12 flex items-center justify-center text-white cursor-pointer hover:bg-yellow-700 ">
                 <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="2" stroke="currentColor" class="w-5 h-5">
                   <path stroke-linecap="round" stroke-linejoin="round" d="M13.5 4.5 21 12m0 0-7.5 7.5M21 12H3" />
                 </svg>
              </div>
            </div>
          </div>
        </div>

        <!-- Arrow Controls (Mobile: ditaruh di bawah carousel) -->
        <div class="flex lg:hidden gap-4 mt-8 items-center cursor-pointer justify-center">
          <div class="w-10 h-10 rounded-full border border-gray-600 flex items-center justify-center hover:bg-gray-800 transition-colors">
            <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="w-4 h-4 text-gray-400">
              <path stroke-linecap="round" stroke-linejoin="round" d="M15.75 19.5 8.25 12l7.5-7.5" />
            </svg>
          </div>
          <div class="w-10 h-10 rounded-full border border-gray-600 flex items-center justify-center hover:bg-gray-800 transition-colors">
            <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="w-4 h-4 text-gray-400">
              <path stroke-linecap="round" stroke-linejoin="round" d="m8.25 4.5 7.5 7.5-7.5 7.5" />
            </svg>
          </div>
        </div>

      </div>

    </div>
  </div>
</template>

<style scoped>
.carousel::-webkit-scrollbar {
  display: none;
}
.carousel {
  -ms-overflow-style: none;
  scrollbar-width: none;
}

.no-scrollbar::-webkit-scrollbar {
  display: none;
}
.no-scrollbar {
  -ms-overflow-style: none;  /* IE and Edge */
  scrollbar-width: none;  /* Firefox */
}
</style>