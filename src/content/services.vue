<template>
  <div class="container mx-auto px-4 mt-60 lg:mt-60">
    <div class="flex flex-col lg:flex-row justify-between items-center mt-12 gap-6">
      <div class="max-w-xs lg:max-w-none">
        <div class="rounded-lg overflow-hidden mb-4 lg:mb-0 hover:scale-105 duration-100 animate-up-down">
          <img src="../assets/img/phoneframecompres.png" alt="" width="800px" />
        </div>
      </div>
      <div class="w-full lg:w-1/2 desk_services">
        <div class="rounded-lg">
          <h3 class="text-3xl font-semibold mb-4">Layanan untuk Pengguna</h3>
          <p class="text-sm mt-10 lg:text-base xl:w-4/5">Lorem, ipsum dolor sit amet consectetur adipisicing elit. Voluptatum cumque ipsum fuga unde. Esse amet rerum reprehenderit asperiores eaque. Qui nisi veritatis laboriosam! Consequatur nihil rem voluptatem sint quia amet sequi impedit corporis sed voluptates. Ipsam quae quo nam! Voluptatibus reiciendis excepturi unde inventore doloribus, nemo hic? Harum, et laboriosam!</p>
          <button class="p-4 bg-gray-900 hover:bg-gray-700 duration-100 rounded-2xl text-gray-200 text-sm w-60 mt-9">
            <a href="#">Dejavu Leave</a>
          </button>
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped>
  @media screen and (max-width: 767px) {
    .desk_services {
      text-align: center;
    }
  }

  @keyframes up-down {
    0% {
      transform: translateY(0);
    }
    50% {
      transform: translateY(-10px);
    }
    100% {
      transform: translateY(0);
    }
  }

  .animate-up-down {
    animation: up-down 2s infinite;
  }
</style>
