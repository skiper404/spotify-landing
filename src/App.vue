<script setup>
import BrowseLogo from "./components/BrowseLogo.vue";
import DownloadLogo from "./components/DownloadLogo.vue";
import HomeLogo from "./components/HomeLogo.vue";
import SearchLogo from "./components/SearchLogo.vue";
import SpotifyLogo from "./components/SpotifyLogo.vue";
</script>

<template>
  <div class="h-screen bg-black text-gray-400">
    <header>
      <nav class="flex items-center justify-between p-2">
        <section class="flex items-center justify-center gap-2">
          <a href="#" class="mx-4">
            <SpotifyLogo class="size-9" />
          </a>
          <a
            href="#"
            class="rounded-full bg-gray-800 p-3 transition duration-150 hover:bg-gray-700"
          >
            <HomeLogo class="size-6" />
          </a>
          <a
            href="#"
            class="rounded-full bg-gray-800 p-3 transition duration-150 hover:bg-gray-700"
          >
            <SearchLogo class="size-6" />
          </a>
        </section>
        <section class="flex items-center justify-between gap-2 font-semibold">
          <ul class="flex items-center justify-between gap-2 px-2">
            <li>Premium</li>
            <li>Support</li>
            <li>Download</li>
          </ul>
          |
          <div class="flex items-center justify-between gap-4">
            <a href="#" class="flex items-center gap-2 px-4"
              ><DownloadLogo class="size-6" />Install App
            </a>
            <div class="flex items-center justify-center gap-4">
              <a href="#">Sign up</a>
              <a
                href="#"
                class="rounded-full bg-gray-100 px-7 py-3 text-gray-900 transition duration-150 hover:scale-105 hover:bg-amber-50"
                >Log in</a
              >
            </div>
          </div>
        </section>
      </nav>
    </header>
    <main class="flex">
      <a
        href="#search"
        class="peer rounded-full bg-gray-800 p-3 transition duration-150 hover:bg-gray-700"
      >
        <SearchLogo class="size-6" />
      </a>
      <div id="search" class="relative peer-focus:block focus-within:block">
        <SearchLogo class="absolute top-3 left-4 size-6" />
        <input type="text" class="w-80 rounded-full border-2 px-12 py-2" />
        <BrowseLogo class="absolute top-3 right-3 size-6" />
      </div>
    </main>
  </div>
</template>

<style lang="scss" scoped></style>
