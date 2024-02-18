<template>
  <div class="grid grid-rows-3 grid-flow-col gap-0 h-full w-full">
    <div
      class="row-span-3 hidden sm:block cols-span-1 bg-cover p-4 bg-[url('https://images.unsplash.com/photo-1600173293426-65190a24be72?q=80&w=1624&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D')]"
    >
      <NuxtLink to="/" class="-m-1.5 p-1.5">
        <p class="font-bold text-2xl text-white">BibleHub.</p>
      </NuxtLink>
    </div>
    <div
      class="row-span-3 p-4 cols-span-2 w-full sm:w-full mx-auto my-auto isolate relative"
    >
      <slot />
    </div>
  </div>
</template>

<script setup lang="ts"></script>

<style scoped></style>
