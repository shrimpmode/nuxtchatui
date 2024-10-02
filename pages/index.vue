<template>
  <div class="p-4">
    <div class="text-2xl mb-4">Title</div>
    <div class="flex flex-col gap-4">
      <div v-for="message in messages" class="">
        <Message />
      </div>
    </div>
  </div>
</template>

<script setup lang="ts">
const messages = ref(Array.from({ length: 10 }, (_, i) => ({ id: i })));
</script>
