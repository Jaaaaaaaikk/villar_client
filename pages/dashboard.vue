<template>
<div>
  <nav class="bg-gray-800">
    <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
      <div class="flex items-center justify-between h-16">
        <div class="flex items-center">
          <div class="flex-shrink-0">
            <h2 class="text-gray-300 hover:bg-gray-700 hover:text-white">Dashboard</h2>
          </div>
          <div class="hidden md:block">
            <div class="ml-10 flex items-baseline space-x-4">
                <NuxtLink to="/dashboard" class="text-gray-300 hover:text-gray-700 px-3 py-2 rounded-md text-sm font-medium">Home</NuxtLink>
              <NuxtLink to="/aboutus" class="text-gray-300 hover:text-gray-700 px-3 py-2 rounded-md text-sm font-medium">About us</NuxtLink>
              <NuxtLink to="/contact" class="text-gray-300 hover:text-gray-700 px-3 py-2 rounded-md text-sm font-medium">Contact</NuxtLink>
              <NuxtLink to="/plans" class="text-gray-300 hover:text-gray-700 px-3 py-2 rounded-md text-sm font-medium">Plans</NuxtLink>
              <NuxtLink to="/faq" class="text-gray-300 hover:text-gray-700 px-3 py-2 rounded-md text-sm font-medium">FAQ</NuxtLink>
            </div>
          </div>
        </div>
        <div class="hidden md:block">
          <div class="ml-4 flex items-center md:ml-6">
            <button class="bg-gray-800 p-1 rounded-full text-gray-400 hover:text-white focus:outline-none focus:ring-2 focus:ring-offset-2 focus:ring-offset-gray-800 focus:ring-white">
              <span class="sr-only">View notifications</span>
              <svg class="h-6 w-6" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke="currentColor" aria-hidden="true">
                <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M15 17h5l-1.405-1.405A2.032 2.032 0 0118 14.158V11a6.002 6.002 0 00-4-5.659V5a2 2 0 10-4 0v.341C7.67 6.165 6 8.388 6 11v3.159c0 .538-.214 1.055-.595 1.436L4 17h5m6 0v1a3 3 0 11-6 0v-1m6 0H9" />
              </svg>
            </button>
          </div>
        </div>
        <div class="-mr-2 flex md:hidden">
          <!-- Mobile menu button -->
          <button class="bg-gray-800 inline-flex items-center justify-center p-2 rounded-md text-gray-400 hover:text-white hover:bg-gray-700 focus:outline-none focus:ring-2 focus:ring-offset-2 focus:ring-offset-gray-800 focus:ring-white">
            <!-- Menu icon -->
            <svg class="block h-6 w-6" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke="currentColor" aria-hidden="true">
              <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 6h16M4 12h16M4 18h16" />
            </svg>
          </button>
        </div>
      </div>
    </div>
  </nav>
</div>
</template>

<script setup lang="ts">

</script>

<style scoped>

</style>