<template>
  <div class="bg-neutral-900 h-screen p-4 md:w-[400px]">
    <div class="flex gap-4 h-full">
      <div class="flex flex-col gap-2">
        <div v-for="item in items">
          <Skeleton class="h-12 w-12 rounded-full" />
        </div>
      </div>
      <div
        class="p-4 bg-neutral-800 flex-1 flex flex-col gap-4 text-neutral-50"
      >
        <div v-for="chat in chats" class="w-full flex">
          <div class="flex gap-4 w-full">
            <div class="text-3xl">#</div>
            <Skeleton class="h-8 w-full" />
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script setup lang="ts">
import Skeleton from "./ui/skeleton/Skeleton.vue";

const items = ref(Array.from({ length: 10 }, (_, i) => ({ id: i })));
const chats = ref(Array.from({ length: 8 }, (_, i) => ({ id: i })));
</script>
