<script setup></script>

<template>
  <div>
    <AppHeader/>
    <div class="container mx-auto p-4">
      <NuxtLink to="/products" class="btn btn--icon mb-4"><Icon name="material-symbols:arrow-back"/>Back</NuxtLink>
      <slot />
    </div>
    <AppFooter/>
  </div>
</template>

<style scoped></style>