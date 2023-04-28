<script lang="ts">
export default {
  setup() {
    useHead({
      titleTemplate: '%s - useHead example',
      bodyAttrs: {
        class: 'test',
      },
    });
    return { dynamic: ref(49) };
  },
  head: {
    title: 'Another title',
  },
};
</script>
<template>
  <div class="bg-red-950">About us</div>
</template>
