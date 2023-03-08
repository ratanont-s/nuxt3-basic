<script lang="ts" setup></script>

<template>
  <header class="backdrop-blur-xl bg-white/30 py-4 border-b sticky top-0">
    <div class="container mx-auto px-4 flex justify-between items-center">
      <NuxtLink to="/" class="font-bold text-4xl text-teal-500">NNT</NuxtLink>
      <button class="btn px-2 py-1 md:hidden"><Icon name="material-symbols:menu" class="w-6 h-6"/></button>
      <div class="hidden md:flex">
        <nav class="flex flex-col md:flex-row md:gap-x-4">
        <NuxtLink to="/" exact-active-class="text-teal-500">Home</NuxtLink>
        <NuxtLink to="/about" exact-active-class="text-teal-500">About</NuxtLink>
        <NuxtLink to="/products" exact-active-class="text-teal-500">Products</NuxtLink>
        <button><Icon name="material-symbols:shopping-cart-outline"/></button>
      </nav>
      </div>
    </div>
  </header>
</template>

<style scoped></style>
