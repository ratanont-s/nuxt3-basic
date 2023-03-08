<script setup>
const { product } = defineProps(['product'])
</script>

<template>
  <NuxtLink :to="`products/${product.id}`" class="card flex-row items-start gap-x-4 h-full">
    <img :src="product.image" :alt="product.title" class="w-3/12 object-contain">
    <div class="flex flex-col justify-between h-full">
      <h5 class="mb-4">{{ product.title }}</h5>
      <p class="font-bold text-right">${{ product.price }}</p>
    </div>
  </NuxtLink>
</template>

<style scoped></style>
