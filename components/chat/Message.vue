<template>
  <div class="flex gap-4 w-[300px]">
    <div>
      <Skeleton class="h-12 w-12 rounded-full" />
    </div>
    <div class="flex flex-col gap-2 flex-1">
      <div class="flex gap-2">
        <Skeleton class="h-3 w-16" />
        <Skeleton class="h-2 w-10 self-end" />
      </div>
      <div>
        <Skeleton class="h-4 w-full" />
      </div>
    </div>
  </div>
</template>
