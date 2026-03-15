<template>
  <div class="top-navbar navbar bg-white border-b border-gray-200 sticky top-0 z-50 px-4 md:px-8 h-auto py-2 md:py-4 relative">
    
    <!-- Bagian Kiri: Menu Icon & Judul Web -->
    <div class="flex-1 flex items-center gap-4 md:gap-8 justify-start">
      <!-- Menu Button (Custom PNG) -->
      <button class="btn btn-square btn-ghost hover:bg-gray-100">
        <img src="/images/Menu.png" alt="Menu" class="w-6 h-auto" />
      </button>
      
      <!-- Judul Web (Left Aligned on the Navbar, but centered text) -->
      <div class="flex flex-col items-center justify-center pointer-events-none md:ml-4">
        <span class="text-xl md:text-2xl font-serif text-gray-800 tracking-widest uppercase mb-1">PAN PACIFIC</span>
        <span class="text-[8px] md:text-[10px]  text-gray-500 tracking-widest uppercase leading-none">SUZHOU</span>
      </div>
    </div>

    <!-- Bagian Kanan: User & Book Now -->
    <div class="hidden lg:flex flex-none gap-6 items-center">
      <!-- Label Pan Pacific Discovery -->
      <div class="flex items-center gap-2 text-xs md:text-sm">
        <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="w-5 h-5 text-[#b89441]">
          <path stroke-linecap="round" stroke-linejoin="round" d="M17.982 18.725A7.488 7.488 0 0 0 12 15.75a7.488 7.488 0 0 0-5.982 2.975m11.963 0a9 9 0 1 0-11.963 0m11.963 0A8.966 8.966 0 0 1 12 21a8.966 8.966 0 0 1-5.982-2.275M15 9.75a3 3 0 1 1-6 0 3 3 0 0 1 6 0Z" />
        </svg>
        <span class="font-bold text-gray-800 mr-2">Pan Pacific DISCOVERY</span>
        <span class="text-[#b89441] cursor-pointer hover:underline font-bold">Join</span>
        <span class="text-gray-400">|</span>
        <span class="text-[#b89441] cursor-pointer hover:underline font-bold">Sign In</span>
      </div>

      <!-- Tombol Dine With Us -->
      <button class="flex items-center gap-2 px-6 py-2 md:py-3 border border-[#b89441] rounded-full text-[#b89441] font-bold text-[10px] md:text-xs tracking-widest uppercase hover:bg-yellow-50">
        <!-- Ikon Kubah / Cloche -->
        <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="w-4 h-4 md:w-5 md:h-5">
          <path stroke-linecap="round" stroke-linejoin="round" d="M14.857 17.082a23.848 23.848 0 0 0 5.454-1.31A8.967 8.967 0 0 1 18 9.75V9A6 6 0 0 0 6 9v.75a8.967 8.967 0 0 1-2.312 6.022c1.733.64 3.56 1.085 5.455 1.31m5.714 0a24.255 24.255 0 0 1-5.714 0m5.714 0a3 3 0 1 1-5.714 0" />
        </svg>
        DINE WITH US
      </button>

      <!-- Tombol Book Now -->
      <button class="flex items-center gap-2 px-8 py-3 border border-[#b89441] bg-[#f8f5f0] rounded-full text-[#b89441] font-bold text-xs tracking-widest uppercase hover:bg-yellow-50 shadow-sm">
        <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="w-5 h-5">
           <path stroke-linecap="round" stroke-linejoin="round" d="M2.25 12l8.954-8.955c.44-.439 1.152-.439 1.591 0L21.75 12M4.5 9.75v10.125c0 .621.504 1.125 1.125 1.125H9.75v-4.875c0-.621.504-1.125 1.125-1.125h2.25c.621 0 1.125.504 1.125 1.125V21h4.125c.621 0 1.125-.504 1.125-1.125V9.75M8.25 21h8.25" />
        </svg>
        BOOK NOW
      </button>
    </div>

  </div>
</template>