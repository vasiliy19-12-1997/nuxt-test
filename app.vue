<script setup></script>
<template>
  <NuxtExampleLayout example="routing/pages">
    <NuxtLoadingIndicator />
    <NuxtPage />
    <template #nav>
      <nav class="flex align-center gap-4 p-4">
        <NuxtLink to="/" class="n-link-base"> Home </NuxtLink>
        <NuxtLink to="/about" class="n-link-base"> About </NuxtLink>
      </nav>
    </template>
  </NuxtExampleLayout>
</template>
