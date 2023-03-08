<script setup>
const { data } = await useFetch('/api/currency/THB')
</script>

<template>
  <div>
    <h1 class="font-bold text-4xl mb-4">About</h1>
    <p>Lorem ipsum dolor, sit amet consectetur adipisicing elit. Expedita sed similique esse temporibus sunt architecto consequuntur doloribus fugit ut, at eligendi odit tenetur quas, soluta labore voluptatum adipisci, fuga pariatur.</p>
    <p>{{ data }}</p>
  </div>
</template>

<style scoped></style>
