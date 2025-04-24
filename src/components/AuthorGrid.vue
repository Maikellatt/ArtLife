<template>
  <section class="px-6 md:px-12 py-16 max-w-7xl mx-auto">
    <h2 class="text-3xl font-bold mb-6">AUTHORS</h2>
    <div class="grid md:grid-cols-3 gap-6">
      <div v-for="a in authors" :key="a.name" class="flex items-center gap-4 border p-4">
        <img :src="a.image" class="w-12 h-12 rounded-full object-cover" />
        <div>
          <p class="font-semibold">{{ a.name }}</p>
          <p class="text-sm text-gray-500">{{ a.role }}</p>
        </div>
      </div>
    </div>
  </section>
</template>

<script setup>
const authors = [
  { name: 'Jakob Grønborg', role: 'Art Journalist', image: 'https://i.pravatar.cc/100?img=1' },
  { name: 'Jane Cooper', role: 'Critic', image: 'https://i.pravatar.cc/100?img=2' },
  { name: 'Louise Jensen', role: 'Editor', image: 'https://i.pravatar.cc/100?img=3' },
  { name: 'Anna Nielsen', role: 'Writer', image: 'https://i.pravatar.cc/100?img=4' },
  { name: 'Anne Henry', role: 'Illustrator', image: 'https://i.pravatar.cc/100?img=5' },
  { name: 'Cristofer Voearo', role: 'Photographer', image: 'https://i.pravatar.cc/100?img=6' },
]
</script>
