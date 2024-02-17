<template>
  <div class="grid grid-rows-3 grid-flow-col gap-0 h-screen max-w-screen-sm">
    <div class="row-span-3 cols-span-1 bg-black sm:hidden"></div>
    <div
      class="row-span-3 p-4 cols-span-2 lg:w-1/2 md:w-3/5 sm:w-full mx-auto max-w-screen-sm my-auto"
    >
      <slot />
    </div>
  </div>
</template>

<script setup lang="ts"></script>

<style scoped></style>
