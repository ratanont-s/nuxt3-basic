<script setup>
const { pending, data: products } = useLazyFetch('https://fakestoreapi.com/products')
</script>

<template>
  <div>
    <h1 class="font-bold text-4xl mb-4">Products</h1>
    <p class="mb-4">Lorem ipsum dolor sit, amet consectetur adipisicing elit. Voluptatem delectus ipsam dolore quasi, dolorem omnis reprehenderit, numquam doloribus similique, ducimus excepturi adipisci et officia ipsa. Ipsum est dolor quae id.</p>
    <div v-if="pending">
      <p class="text-teal-500 text-center py-10">Loading...</p>
    </div>
    <ul v-else class="grid grid-cols-1 gap-4 sm:grid-cols-2 lg:grid-cols-3">
      <li v-for="p in products">
        <ProductCard :product="p"/>
      </li>
    </ul>
  </div>
</template>

<style scoped></style>
