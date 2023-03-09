<script lang="ts" setup></script>

<template>
  <div class="flex flex-col min-h-screen">
    <AppHeader/>
    <div class="container mx-auto px-4 py-8 md:px-8 md:py-16">
      <slot />
    </div>
    <AppFooter/>
  </div>
</template>

<style scoped></style>
