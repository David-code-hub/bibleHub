<template>
  <div>
    <div class="px-6 pt-14 lg:px-8">
      <div class="mx-auto max-w-2xl py-32 sm:py-48 lg:py-56">
        <div class="text-left">
          <div class="hidden sm:mb-4 sm:flex">
            <div
              class="relative rounded-xl py-1 text-sm leading-6 text-gray-600 ring-0 ring-gray-900/10 hover:ring-gray-900/20"
            >
              <i class="bi bi-heart-fill mr-1.5 text-black"></i> Share your
              Christian walk with other believers.
            </div>
          </div>
          <h1 class="text-4xl font-bold tracking-tight sm:text-6xl text-black">
            BibleHub.
          </h1>
          <p
            class="-mx-3 px-3 mt-4 text-base font-normal leading-7 text-gray-900"
          >
            For God so loved the world, that he gave his only begotten Son, that
            whosoever believeth in him should not perish, but have everlasting
            life.
          </p>
          <p class="w-full font-normal text-sm">- John 3:16</p>
          <div class="mt-10 flex items-left justify-left">
            <NuxtLink to="/" class="btn btn-bg-dark py-4 px-6"
              >Explore More <i class="bi bi-arrow-right ml-1.5"></i
            ></NuxtLink>
            <NuxtLink to="/account/signup" class="btn py-4 px-6"
              >Create Your Account <i class="bi bi-person-plus-fill ml-1.5"></i
            ></NuxtLink>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script setup lang="ts"></script>
