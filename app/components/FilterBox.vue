<template>

    <!-- COMPONENT: FilterBox.vue                 -->
    
    <!-- ini kotak melayang yg ada dropdownnya -->
    <div class="filter-box lg:hidden fixed bottom-4 left-1/2 -translate-x-1/2 z-50 w-[90%] max-w-sm rounded-full bg-[#3d3935] p-2 flex gap-2 shadow-2xl items-center border border-gray-600">
      
      <!-- Tombol Kiri -->
      <button class="flex-1 bg-[#f3efe8] rounded-full py-2 px-4 flex justify-between items-center text-left">
        <div class="flex items-center gap-2">
          <!-- Icon user -->
          <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="w-5 h-5 text-gray-700">
            <path stroke-linecap="round" stroke-linejoin="round" d="M15.75 6a3.75 3.75 0 1 1-7.5 0 3.75 3.75 0 0 1 7.5 0ZM4.501 20.118a7.5 7.5 0 0 1 14.998 0A17.933 17.933 0 0 1 12 21.75c-2.676 0-5.216-.584-7.499-1.632Z" />
          </svg>
          <div>
            <p class="text-[10px] text-gray-500 leading-none">Who's exploring</p>
            <p class="text-sm font-bold text-gray-800 leading-tight">All travellers</p>
          </div>
        </div>
        <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="2" stroke="currentColor" class="w-4 h-4 text-yellow-600">
          <path stroke-linecap="round" stroke-linejoin="round" d="m19.5 8.25-7.5 7.5-7.5-7.5" />
        </svg>
      </button>

      <!-- Tombol Kanan -->
      <button class="flex-1 bg-[#f3efe8] rounded-full py-2 px-4 flex justify-between items-center text-left">
        <div class="flex items-center gap-2">
          <!-- Icon pin -->
          <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="w-5 h-5 text-gray-700">
            <path stroke-linecap="round" stroke-linejoin="round" d="M15 10.5a3 3 0 1 1-6 0 3 3 0 0 1 6 0Z" />
            <path stroke-linecap="round" stroke-linejoin="round" d="M19.5 10.5c0 7.142-7.5 11.25-7.5 11.25S4.5 17.642 4.5 10.5a7.5 7.5 0 1 1 15 0Z" />
          </svg>
          <div>
            <p class="text-[10px] text-gray-500 leading-none">Your journey to</p>
            <p class="text-sm font-bold text-gray-800 leading-tight">Anywhere</p>
          </div>
        </div>
        <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="2" stroke="currentColor" class="w-4 h-4 text-yellow-600">
          <path stroke-linecap="round" stroke-linejoin="round" d="m19.5 8.25-7.5 7.5-7.5-7.5" />
        </svg>
      </button>

    </div>
    <!-- END COMPONENT -->
</template>

<script setup>
// State dropdown/filter bisa dilanjutkan di sini jika butuh interaktivitas
</script>