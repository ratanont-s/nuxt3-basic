<script setup>
const { product } = defineProps(['product'])
</script>

<template>
  <div class="bg-white p-4 rounded grid grid-cols-1 gap-4 md:grid-cols-5 md:gap-8">
    <div class="col-span-2">
      <img :src="product.image" :alt="product.title">
    </div>
    <div class="col-span-3 flex flex-col">
      <h1 class="font-bold text-xl mb-2">{{ product.title }}</h1>
      <p class="mb-4"><span class="bg-teal-500 text-white text-sm px-2 py-1 rounded">{{ product.category }}</span></p>
      <p class="mb-4">{{ product.description }}</p>
      <p class="mt-8">Price: <span class="font-bold text-xl">${{ product.price }}</span></p>
    </div>
  </div>
</template>

<style scoped></style>
