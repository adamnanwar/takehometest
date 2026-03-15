<template>

<!-- COMPONENT: EditorChoise.vue                -->

  <div class="editor-pick-responsive bg-[#f4f0e6] text-[#24211f] flex flex-col justify-center items-center pt-12 lg:pt-16 pb-0 relative z-10">
    
    <!-- Bagian Judul Utama (Header) - Tengah pada Mobile & Desktop -->
    <div class="w-full flex flex-col items-center mb-8">
      <!-- Icon Mahkota -->
      <div class="bg-[#a39478] rounded-full w-12 h-12 flex items-center justify-center text-white mb-4">
         <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="w-6 h-6">
          <path stroke-linecap="round" stroke-linejoin="round" d="M11.48 3.499a.562.562 0 0 1 1.04 0l2.125 5.111a.563.563 0 0 0 .475.345l5.518.442c.499.04.701.663.321.988l-4.204 3.602a.563.563 0 0 0-.182.557l1.285 5.385a.562.562 0 0 1-.84.61l-4.725-2.885a.562.562 0 0 0-.586 0L6.982 20.54a.562.562 0 0 1-.84-.61l1.285-5.386a.562.562 0 0 0-.182-.557l-4.204-3.602a.562.562 0 0 1 .321-.988l5.518-.442a.563.563 0 0 0 .475-.345L11.48 3.5Z" />
        </svg>
      </div>
      <h2 class="font-serif text-5xl md:text-6xl text-center">Editor's pick</h2>
    </div>

    <!-- Container Konten Utama: Terbagi 2 kolom pada Desktop -->
    <!-- mx-auto dan batasan lebar agar rapih pada desktop -->
    <div class="w-full max-w-6xl mx-auto flex flex-col lg:flex-row items-center justify-between px-6 lg:px-10 gap-8 lg:gap-20">
      
      <!-- Bagian Gambar Kiri (Desktop) & Bawah (Mobile) -->
      <!-- Di Mobile urutan flex-col-reverse atau defaultnya gambar di bawah, Teks di atas -->
      <div class="w-full lg:w-1/2 order-2 lg:order-1 relative z-20">
         <img src="/images/cocktail.png" alt="Cocktail" class="w-full h-auto object-cover max-h-[500px] shadow-lg translate-y-8 lg:translate-y-8" />
      </div>

      <!-- Bagian Teks Kanan (Desktop) & Kiri (Mobile) -->
      <div class="w-full lg:w-1/2 order-1 lg:order-2 flex flex-col items-start text-left mb-8 lg:mb-0 px-4 md:px-10 lg:px-0">
        <p class="text-[9px] md:text-[10px] uppercase tracking-widest font-bold flex items-center justify-start gap-1 mb-6 text-[#8a7238]">
           <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="2" stroke="currentColor" class="w-3.5 h-3.5">
            <path stroke-linecap="round" stroke-linejoin="round" d="M15 10.5a3 3 0 1 1-6 0 3 3 0 0 1 6 0Z" />
            <path stroke-linecap="round" stroke-linejoin="round" d="M19.5 10.5c0 7.142-7.5 11.25-7.5 11.25S4.5 17.642 4.5 10.5a7.5 7.5 0 1 1 15 0Z" />
          </svg>
          AUSTRALIA
        </p>
        
        <h3 class="font-serif text-3xl md:text-4xl leading-tight mb-8">Fun Things to do in Parramatta at Night</h3>
        
        <div class="flex gap-2 flex-wrap justify-start mb-10">
          <span class="border border-[#d6d0c4] text-[#5e584f] text-[9px] py-1.5 px-4 rounded-full uppercase tracking-widest font-semibold cursor-pointer">COUPLE</span>
          <span class="border border-[#d6d0c4] text-[#5e584f] text-[9px] py-1.5 px-4 rounded-full uppercase tracking-widest font-semibold cursor-pointer">TRAVEL GUIDE</span>
          <span class="border border-[#d6d0c4] text-[#5e584f] text-[9px] py-1.5 px-4 rounded-full uppercase tracking-widest font-semibold cursor-pointer mt-1">CITIES & NIGHTLIFE</span>
          <span class="border border-[#d6d0c4] text-[#5e584f] text-[9px] py-1.5 px-4 rounded-full uppercase tracking-widest font-semibold cursor-pointer mt-1">ROMANCE</span>
        </div>

        <a href="#" class="text-[#a88a42] text-sm hover:underline flex items-center justify-start gap-2 font-serif">
          Read more <span class="not-italic text-lg leading-none">&rarr;</span>
        </a>
      </div>

    </div>

    <!-- Kotak Gelap Bawah (Hanya untuk memberi background gelap / melanjutkan bg section berikutnya) -->
    <div class="w-full h-32 md:h-40 bg-[#24211f] absolute bottom-0 left-0 -z-0"></div>
    
  </div>
</template>