<script setup>
defineProps(['error'])

const handleError = () => clearError({ redirect: '/' })
</script>

<template>
    <div class="w-screen h-screen flex flex-col justify-center items-center text-center">
        <h1 class="font-bold text-8xl mb-4">{{ error.statusCode }}</h1>
        <p class="mb-10">{{ error.message }}</p>
        <button class="btn btn--primary" @click="handleError">Go back Home</button>
    </div>
</template>

<style scoped></style>