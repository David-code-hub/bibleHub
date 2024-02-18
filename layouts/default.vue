<template>
  <div class="relative isolate bg-white">
    <div
      class="absolute inset-x-0 -top-40 -z-10 transform-gpu overflow-hidden blur-3xl sm:-top-80"
      aria-hidden="true"
    >
      <div
        class="bg-gradient-top"
        style="
          clip-path: polygon(
            74.1% 44.1%,
            100% 61.6%,
            97.5% 26.9%,
            85.5% 0.1%,
            80.7% 2%,
            72.5% 32.5%,
            60.2% 62.4%,
            52.4% 68.1%,
            47.5% 58.3%,
            45.2% 34.5%,
            27.5% 76.7%,
            0.1% 64.9%,
            17.9% 100%,
            27.6% 76.8%,
            76.1% 97.7%,
            74.1% 44.1%
          );
        "
      />
    </div>
    <header class="absolute inset-x-0 top-0 z-50">
      <nav
        class="flex items-center justify-between px-6 py-4 lg:px-8 bg-white shadow"
        aria-label="Global"
      >
        <div class="flex lg:flex-1">
          <NuxtLink to="/" class="-m-1.5 p-1.5">
            <p class="font-bold text-2xl">BibleHub.</p>
          </NuxtLink>
        </div>
        <div class="flex lg:hidden">
          <button
            type="button"
            class="-m-2.5 inline-flex items-center justify-center rounded-md p-2.5 text-gray-700"
            @click="mobileMenuOpen = true"
          >
            <span class="sr-only">Open main menu</span>
            <Bars3Icon class="h-6 w-6" aria-hidden="true" />
          </button>
        </div>
        <div class="hidden lg:flex lg:gap-x-12">
          <NuxtLink class="text-sm font-semibold leading-6 text-gray-900"
            ><i class="bi bi-people-fill mr-1.5"></i> Our Community</NuxtLink
          >
          <NuxtLink class="text-sm font-semibold leading-6 text-gray-900"
            ><i class="bi bi-discord mr-1.5"></i>Connect With Us</NuxtLink
          >
          <a
            href="https://github.com/David-code-hub/bibleHub"
            target="_blank"
            class="text-sm font-semibold leading-6 text-gray-900"
            ><i class="bi bi-github mr-1.5"></i> Github Repo</a
          >
        </div>

        <div class="hidden lg:flex lg:flex-1 lg:justify-end">
          <NuxtLink to="/account/signup" class="btn">Sign Up</NuxtLink>
          <NuxtLink to="/account/login" class="btn btn-bg-dark"
            >Log In</NuxtLink
          >
        </div>
      </nav>
      <Dialog
        as="div"
        class="lg:hidden"
        @close="mobileMenuOpen = false"
        :open="mobileMenuOpen"
      >
        <div class="fixed inset-0 z-50" />
        <DialogPanel
          class="fixed inset-y-0 right-0 z-50 w-full overflow-y-auto bg-white px-6 py-6 sm:max-w-sm sm:ring-1 sm:ring-gray-900/10"
        >
          <div class="flex items-center justify-between">
            <a href="#" class="-m-1.5 p-1.5">
              <p class="font-bold mb-6">BibleHub</p>
            </a>
            <button
              type="button"
              class="-m-2.5 rounded-md p-2.5 text-gray-700"
              @click="mobileMenuOpen = false"
            >
              <span class="sr-only">Close menu</span>
              <XMarkIcon class="h-6 w-6" aria-hidden="true" />
            </button>
          </div>
          <div class="mt-0 flow-root">
            <div class="mb-6 divide-y divide-gray-500/10">
              <a href="#" class="btn grid my-3 grid-cols-4 w-3/4">Sign Up</a>
              <a href="#" class="btn btn-bg-dark grid my-3 w-3/4">Log In</a>
              <br />
              <div class="pt-4">
                <p
                  class="-mx-3 px-3 py-2.5 italic text-sm font-normal leading-7 text-gray-700 hover:bg-gray-50"
                >
                  For God so loved the world, that he gave his only begotten
                  Son, that whosoever believeth in him should not perish, but
                  have everlasting life.
                </p>
                <p
                  class="w-full text-right italic font-normal text-gray-600 text-sm"
                >
                  John 3:16
                </p>
              </div>
            </div>
          </div>
        </DialogPanel>
      </Dialog>
    </header>

    <div class="grid grid-cols-2 gap-4 h-full w-full max-w-screen-2xl mx-auto">
      <div
        class="bg-cover bg-[url('https://images.unsplash.com/photo-1600173293426-65190a24be72?q=80&w=1624&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D')]"
      ></div>
      <div class="p-4 w-full sm:w-full mx-auto my-auto">
        <slot />
      </div>
    </div>
    <!-- <slot /> -->
  </div>
</template>

<script setup>
const mobileMenuOpen = ref(false);
</script>

<style scoped></style>
