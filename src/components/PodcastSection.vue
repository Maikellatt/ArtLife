<template>
  <section class="bg-white px-6 md:px-12 py-16 max-w-7xl mx-auto">
    <h2 class="text-3xl font-bold mb-6">PODCAST</h2>
    <div class="grid md:grid-cols-3 gap-6">
      <div v-for="n in 3" :key="n" class="bg-gray-100 p-4">
        <img src="../assets/podcast-cover.png" class="w-full" />
        <h4 class="text-xl mt-4 font-semibold">Episode Title {{ n }}</h4>
        <p class="text-sm text-gray-600 mt-1">Subtitle or guest name</p>
      </div>
    </div>
  </section>
</template>
