<template>
  <div class="grid grid-rows-3 grid-flow-col gap-0 h-screen">
    <div
      class="row-span-3 p-4 lg:w-full md:w-4/5 sm:w-full mx-auto max-w-screen-sm my-auto"
    >
      <div class="lg:w-3/4 md:w-full mx-auto mb-1">
        <h2 class="text-2xl font-semibold text-gray-900">
          Log In to BibleHub.
        </h2>
      </div>

      <form class="lg:w-3/4 md:w-full mx-auto border-b border-gray-900/10">
        <div>
          <label for="email" class="form-field-label">Email address</label>
          <div class="mt-2">
            <input
              id="email"
              name="email"
              type="email"
              placeholder="johndoe@gmail.com"
              autocomplete="email"
              required
              class="form-input-field"
            />
          </div>
        </div>

        <div>
          <div class="flex items-center justify-between">
            <label for="password" class="form-field-label">Password</label>
          </div>
          <div class="mt-2">
            <input
              id="password"
              name="password"
              type="password"
              placeholder="********"
              autocomplete="current-password"
              required
              class="form-input-field"
            />
          </div>
        </div>

        <div>
          <button type="submit" class="btn btn-bg-dark btn-form my-6">
            Log In
          </button>
        </div>
      </form>

      <p class="mt-5 text-center text-sm text-gray-500">
        Don't have an account?
        <NuxtLink
          to="/account/signup"
          class="font-semibold leading-6 text-[#0d1321]"
          >Sign Up</NuxtLink
        >
      </p>
    </div>
  </div>
</template>

<script setup>
definePageMeta({
  layout: "account",
});
</script>

<style scoped></style>
