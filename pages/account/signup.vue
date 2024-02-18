<template>
  <div class="grid grid-rows-3 grid-flow-col gap-0 h-screen">
    <div class="row-span-3 p-4 w-full md:w-4/5 mx-auto max-w-screen-sm my-auto">
      <div class="lg:w-3/4 md:w-full mx-auto mb-1">
        <h2 class="text-2xl font-semibold text-gray-900">
          Sign Up to BibleHub.
        </h2>
      </div>

      <form class="lg:w-3/4 md:w-full mx-auto border-b border-gray-900/10">
        <div class="mt-1 grid grid-cols-1 gap-x-6 gap-y-8 sm:grid-cols-6">
          <div class="sm:col-span-3">
            <label for="first-name" class="form-field-label">First name</label>
            <div class="mt-2">
              <input
                type="text"
                name="first-name"
                placeholder="John"
                id="first-name"
                autocomplete="given-name"
                class="form-input-field"
              />
            </div>
          </div>

          <div class="sm:col-span-3">
            <label for="last-name" class="form-field-label">Last name</label>
            <div class="mt-2">
              <input
                type="text"
                name="last-name"
                placeholder="Doe"
                id="last-name"
                autocomplete="family-name"
                class="form-input-field"
              />
            </div>
          </div>
        </div>

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
          <label for="favourite_bible_verse" class="form-field-label"
            >Your Favourite Bible Verse</label
          >
          <div class="mt-2">
            <input
              id="email"
              name="favourite-bible-verse"
              type="text"
              placeholder="Pslam 23:1"
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
          <div class="flex items-center justify-between">
            <label for="password" class="form-field-label"
              >Confirm Password</label
            >
          </div>
          <div class="mt-2">
            <input
              id="confirm-password"
              name="confirm-password"
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
            Sign Up
          </button>
        </div>
      </form>

      <p class="mt-5 text-center text-sm text-gray-500">
        Already have an account?
        <NuxtLink to="/account/login" class="font-semibold text-[#0d1321]"
          >Log In</NuxtLink
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
