<template>
    <div class="p-4">
      <h1 class="text-2xl font-bold mb-4">All Blog Posts</h1>
  
      <div v-for="post in posts" :key="post._path" class="mb-4">
        <NuxtLink :to="post._path" class="text-blue-500 underline">
          {{ post.title }}
        </NuxtLink>
        <p class="text-gray-600 text-sm">{{ post.description }}</p>
        <p class="text-gray-400 text-xs">{{ post.date }}</p>
      </div>
    </div>
  </template>
  
  <script setup>
  // Load posts
  const { data: posts } = await useAsyncData('posts', () =>
    queryContent('/blog').sort({ date: -1 }).find()
  )
  </script>
  