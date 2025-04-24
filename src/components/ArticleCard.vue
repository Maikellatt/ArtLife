<template>
  <div class="flex gap-6">
    <img :src="image" class="w-32 h-32 object-cover rounded" />
    <div>
      <h3 class="text-xl font-bold">{{ title }}</h3>
      <p class="text-gray-600 text-sm mt-1">{{ desc }}</p>
      <p class="text-gray-500 text-xs mt-2">By {{ author }}</p>
    </div>
  </div>
</template>

<script setup>
defineProps(['title', 'desc', 'author', 'image'])
</script>
