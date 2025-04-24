<template>
  <div class="flex items-center justify-center pt-12">
    <div class="w-full max-w-xl bg-white rounded-2xl shadow-lg p-8">
      <h1 class="text-3xl font-semibold text-gray-800 mb-6 text-center">Contact Us</h1>

      <form @submit.prevent="submitForm" class="space-y-4">
        <div>
          <label class="block text-gray-700 font-medium mb-1" for="name">Name</label>
          <input v-model="form.name" id="name" type="text" required
            class="w-full px-4 py-2 border border-gray-300 rounded-xl focus:ring-2 focus:ring-blue-400 focus:outline-none" />
        </div>

        <div>
          <label class="block text-gray-700 font-medium mb-1" for="email">Email</label>
          <input v-model="form.email" id="email" type="email" required
            class="w-full px-4 py-2 border border-gray-300 rounded-xl focus:ring-2 focus:ring-blue-400 focus:outline-none" />
        </div>

        <div>
          <label class="block text-gray-700 font-medium mb-1" for="message">Message</label>
          <textarea v-model="form.message" id="message" rows="4" required
            class="w-full px-4 py-2 border border-gray-300 rounded-xl focus:ring-2 focus:ring-blue-400 focus:outline-none"></textarea>
        </div>

        <button type="submit"
          class="w-full bg-blue-600 text-white py-2 rounded-xl hover:bg-blue-700 transition">
          Send Message
        </button>
      </form>
    </div>
  </div>
</template>

<script setup>
import { reactive } from 'vue'

const form = reactive({
  name: '',
  email: '',
  message: ''
})

const submitForm = () => {
  // For now just log it
  console.log('Form submitted:', form)

  // Optionally reset form
  form.name = ''
  form.email = ''
  form.message = ''
}
</script>
