<script setup>
const isOpen = ref(false)
</script>

<template>
  <header class="bg-white py-4 border-b sticky top-0 md:py-2">
    <div class="container mx-auto px-4 flex justify-between items-center">
      <NuxtLink to="/" class="font-bold text-4xl text-teal-500">NNT</NuxtLink>
      <button class="btn px-2 py-1 md:hidden" @click="isOpen = !isOpen">
        <Icon name="material-symbols:menu" class="w-6 h-6" />
      </button>
      <div :class="isOpen ? 'fixed top-16 left-0 right-0 bg-white shadow-xl py-2 md:inline-block md:py-0 md:static md:bg-transparent md:shadow-none' : 'hidden md:inline-block'">
        <nav class="flex flex-col md:flex-row" @click="isOpen = !isOpen">
          <NuxtLink to="/" class="px-4 py-2" exact-active-class="text-teal-500">Home</NuxtLink>
          <NuxtLink to="/about" class="px-4 py-2" exact-active-class="text-teal-500">About</NuxtLink>
          <NuxtLink to="/products" class="px-4 py-2" exact-active-class="text-teal-500">Products</NuxtLink>
        </nav>
      </div>
    </div>
  </header>
</template>

<style scoped></style>
