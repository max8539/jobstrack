<script setup lang="ts">
  defineProps<{
    message: string
  }>()
</script>

<template>
  <div
    class="rounded-md bg-red-100 dark:bg-red-900 border-2 border-red-500 text-slate-800 dark:text-slate-200 transition-opacity duration-300"
    :class="message !== '' ? 'opacity-1' : 'opacity-0'"
  >
    
    <div class="p-2">
      {{ message }}
    </div>
  </div>
</template>