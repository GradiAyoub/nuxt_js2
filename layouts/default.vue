<template>
    <div>
      <!-- Header Section -->
      <header class="bg-blue-600 text-white p-4">
        <div class="container mx-auto flex justify-between items-center">
          <h1 class="text-xl font-bold">My Affiliate Site</h1>
          <nav>
            <ul class="flex space-x-4">
              <li>
                <NuxtLink to="/" class="hover:underline">Home</NuxtLink>
              </li>
              <li>
                <NuxtLink to="/page1" class="hover:underline">Page 1</NuxtLink>
              </li>
              <li>
                <NuxtLink to="/posts" class="hover:underline">posts</NuxtLink>
              </li>
              <li>
                <NuxtLink to="/conts" class="hover:underline">conts</NuxtLink>
              </li>
              
            </ul>
          </nav>
        </div>
      </header>
  
      <!-- Main Content (this will be replaced with the page content) -->
      <main class="container mx-auto p-4">
        <NuxtPage />
      </main>
  
      <!-- Footer Section (optional) -->
      <footer class="bg-gray-800 text-white text-center p-4 mt-4">
        <p>&copy; 2025 My Affiliate Site. All rights reserved.</p>
      </footer>
    </div>
  </template>
  
  <script setup>
  // No JavaScript needed for this simple layout
  </script>
  
  <style scoped>
  /* Optional custom styles */
  </style>
  