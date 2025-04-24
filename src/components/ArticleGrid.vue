<template>
  <section class="max-w-7xl mx-auto py-12 grid md:grid-cols-3 gap-12">
    <!-- Articles -->
    <div class="md:col-span-2 space-y-12">
      <ArticleCard
        v-for="(a, i) in articles"
        :key="i"
        :title="a.title"
        :desc="a.desc"
        :author="a.author"
        :image="a.image"
        :date="a.date"
        :readTime="a.readTime"
        :tag="a.tag"
      />

      <div class="text-sm text-blue-600 font-medium underline cursor-pointer">
        → ALL ARTICLES
      </div>
    </div>

    <!-- Sidebar -->
    <aside class="space-y-12">
      <div class="bg-gray-100 p-6">
        <h3 class="text-sm uppercase text-gray-600 mb-2">Printmagazine</h3>
        <p class="text-3xl font-semibold mb-2">03/2022</p>
        <img src="../assets/mojtaba-mosayebzadeh-V9mVXYKGyxc-unsplash 1.png" class="w-full rounded" />
        <button class="mt-4 bg-black text-white px-4 py-2 w-full">Button</button>
      </div>

      <div>
        <h4 class="font-semibold text-lg mb-4">Most Popular</h4>
        <ul class="space-y-3 text-sm">
          <li><strong>01</strong> Street art festival</li>
          <li><strong>02</strong> Hope dies last</li>
          <li><strong>03</strong> Artists who want to rise above</li>
        </ul>
      </div>

      <div>
        <h4 class="font-semibold text-lg mb-2">Newsletter</h4>
        <input type="email" placeholder="Email" class="w-full border p-2 mb-2" />
        <button class="bg-black text-white px-4 py-2 w-full">Sign Up</button>
      </div>
    </aside>
  </section>
</template>

<script setup>
import ArticleCard from './ArticleCard.vue'

const articles = [
  {
    title: 'Hope dies last',
    desc: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Egestas dui id ornare arcu odio ut sem. Cras ornare arcu dui vivamus arcu felis bibendum ut. Porttitor leo a diam.',
    author: 'Jakob Grønborg',
    image: 'https://picsum.photos/200/300',
    date: '16. March 2022',
    readTime: '1 Min',
    tag: 'ART'
  },
  {
    title: 'The best art museums',
    desc: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Egestas dui id ornare arcu odio ut sem. Cras ornare arcu dui vivamus arcu felis bibendum ut. Porttitor leo a diam.',
    author: 'Jakob Grønborg',
    image: 'https://picsum.photos/200/300',
    date: '16. March 2022',
    readTime: '1 Min',
    tag: 'SCULPTURES'
  },
  {
    title: 'The devil is the details',
    desc: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Egestas dui id ornare arcu odio ut sem. Cras ornare arcu dui vivamus arcu felis bibendum ut. Porttitor leo a diam.',
    author: 'Jakob Grønborg',
    image: 'https://picsum.photos/200/300',
    date: '16. March 2022',
    readTime: '1 Min',
    tag: 'ART'
  },
  {
    title: 'An indestructible hope',
    desc: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Egestas dui id ornare arcu odio ut sem. Cras ornare arcu dui vivamus arcu felis bibendum ut. Porttitor leo a diam.',
    author: 'Jakob Grønborg',
    image: 'https://picsum.photos/200/300',
    date: '16. March 2022',
    readTime: '1 Min',
    tag: 'ART'
  },
  {
    title: 'Street art festival',
    desc: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Egestas dui id ornare arcu odio ut sem. Cras ornare arcu dui vivamus arcu felis bibendum ut. Porttitor leo a diam.',
    author: 'Jakob Grønborg',
    image: 'https://picsum.photos/200/300',
    date: '16. March 2022',
    readTime: '1 Min',
    tag: 'STREET ART'
  },
  {
    title: 'Through the eyes of street artists',
    desc: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Egestas dui id ornare arcu odio ut sem. Cras ornare arcu dui vivamus arcu felis bibendum ut. Porttitor leo a diam.',
    author: 'Jakob Grønborg',
    image: 'https://picsum.photos/200/300',
    date: '16. March 2022',
    readTime: '1 Min',
    tag: 'STREET ART'
  }
]
</script>
