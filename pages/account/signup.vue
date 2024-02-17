<template>
  <div class="grid grid-rows-3 grid-flow-col gap-0 h-screen bg-[#F0F3F9]">
    <div
      class="row-span-3 p-4 lg:w-1/2 md:w-3/5 sm:w-full mx-auto max-w-screen-sm my-auto"
    >
      <!-- <p class="font-bold text-2xl">BibleHub.</p> -->

      <div class="lg:w-3/4 md:w-full mx-auto border-b border-gray-900/10 mb-1">
        <h2 class="text-2xl font-normal text-gray-900">Create Your Account</h2>
        <p class="mt-1 text-sm font-light leading-6 text-gray-600 mb-5">
          Join the community and share you walk with us!
        </p>
      </div>

      <form class="lg:w-3/4 md:w-full mx-auto">
        <div class="mt-1 grid grid-cols-1 gap-x-6 gap-y-8 sm:grid-cols-6">
          <div class="sm:col-span-3">
            <label for="first-name" class="form-field-label">First name</label>
            <div class="mt-2">
              <input
                type="text"
                name="first-name"
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
              autocomplete="email"
              required
              class="form-input-field"
            />
          </div>
        </div>

        <div class="col-span-full">
          <label for="about" class="form-field-label">Bio</label>
          <div class="mt-2">
            <textarea
              id="about"
              name="about"
              rows="3"
              class="form-input-field"
            ></textarea>
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
              autocomplete="current-password"
              required
              class="form-input-field"
            />
          </div>
        </div>

        <div>
          <button type="submit" class="btn btn-bg-dark my-6">Sign Up</button>
        </div>
      </form>

      <p class="mt-10 text-center text-sm text-gray-500">
        Already have an account?
        <Nuxtlink
          to="/account/login"
          class="font-semibold leading-6 text-[#0d1321]"
          >Log In</Nuxtlink
        >
      </p>
    </div>
  </div>
</template>

<script setup lang="ts"></script>

<style scoped></style>
