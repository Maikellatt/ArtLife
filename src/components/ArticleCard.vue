<template>
  <div class="flex gap-6">
    <img src="https://picsum.photos/200/300" class="w-90 h-40  rounded" />
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
