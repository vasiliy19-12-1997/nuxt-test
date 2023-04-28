<script setup>
const { data } = await useFetch('http://localhost:3000/posts');
</script>

<template>
  <div v-if="!data?.length">POsts dosnt found</div>
  <ul v-else>
    <li :key="post.id" v-for="(post, index) in data">
      <span v-if="post">{{ index }} - {{ post.title }} {{ post.body }}</span>
      <button :disabled="isLoadingDelete" @click="mutate(post.id)">X</button>
    </li>
  </ul>
</template>
