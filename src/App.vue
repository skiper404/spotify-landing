<script setup>
import BrowseLogo from "./components/BrowseLogo.vue";
import DownloadLogo from "./components/DownloadLogo.vue";
import HomeLogo from "./components/HomeLogo.vue";
import PlusIcon from "./components/PlusIcon.vue";
import SearchLogo from "./components/SearchLogo.vue";
import SpotifyLogo from "./components/SpotifyLogo.vue";
import GlobeIcon from "./components/GlobeIcon.vue";
import BurgerMenu from "./components/BurgerMenu.vue";
import PlayLogo from "./components/PlayLogo.vue";
import InstagramLogo from "./components/InstagramLogo.vue";
import TwitterLogo from "./components/TwitterLogo.vue";
import FacebookLogo from "./components/FacebookLogo.vue";
</script>

<template>
  <div class="bg-[#000000] text-[#aaaaaa]">
    <header class="sticky top-0 z-20 h-16 bg-[#000000]">
      <nav class="flex items-center justify-between p-2">
        <section class="relative flex items-center justify-center gap-2">
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
            href="#search"
            class="rounded-full bg-gray-800 p-3 transition duration-150 hover:bg-gray-700"
          >
            <SearchLogo class="size-6" />
          </a>
          <div id="search" class="absolute top-0.5 left-32 hidden target:block">
            <div>
              <SearchLogo class="absolute top-2.5 left-4 size-6" />
            </div>
            <input
              type="text"
              class="w-100 rounded-full border-2 px-16 py-2 outline-0 placeholder:text-[#a0a0a0]"
              placeholder="What do you want to play?"
            />
            <div>
              <BrowseLogo class="absolute top-2 right-3 size-6" />
            </div>
          </div>
        </section>
        <section class="hidden items-center justify-between lg:flex">
          <ul class="flex items-center justify-between gap-2 px-2 md:flex">
            <li
              class="transition duration-150 hover:scale-105 hover:text-gray-200"
            >
              Premium
            </li>
            <li
              class="transition duration-150 hover:scale-105 hover:text-gray-200"
            >
              Support
            </li>
            <li
              class="transition duration-150 hover:scale-105 hover:text-gray-200"
            >
              Download
            </li>
          </ul>
          |
          <div class="flex items-center justify-between gap-4">
            <a
              href="#"
              class="flex items-center gap-2 px-4 transition duration-150 hover:scale-105 hover:text-gray-200"
              ><DownloadLogo class="h-5" />Install App
            </a>
            <div class="flex items-center justify-center gap-4">
              <a
                href="#"
                class="hover:text-gray transition duration-150 hover:scale-105"
                >Sign up</a
              >
              <a
                href="#"
                class="rounded-full bg-gray-100 px-7 py-3 text-gray-900 transition duration-150 hover:scale-105 hover:bg-amber-50"
                >Log in</a
              >
            </div>
          </div>
        </section>
        <a href="#menu" class="lg:hidden">
          <BurgerMenu class="size-10" />
        </a>
        <div
          class="absolute top-16 right-0 z-40 hidden w-50 bg-gray-950 target:block"
          h-100
          id="menu"
        >
          <ul class="flex flex-col items-center gap-2">
            <li
              class="flex w-full cursor-pointer items-center justify-between px-4 py-2 hover:underline"
            >
              Premium
              <BrowseLogo />
            </li>
            <li
              class="flex w-full items-center justify-between px-4 py-2 hover:underline"
            >
              Support
              <BrowseLogo />
            </li>
            <li
              class="flex w-full items-center justify-between px-4 py-2 hover:underline"
            >
              Download
              <BrowseLogo />
            </li>
            <li
              class="flex w-full items-center justify-between px-4 py-2 hover:underline"
            >
              Sign up
              <BrowseLogo />
            </li>
            <li
              class="flex w-full items-center justify-between px-4 py-2 hover:underline"
            >
              Sign in
              <BrowseLogo />
            </li>
          </ul>
        </div>
      </nav>
    </header>
    <main class="grid max-w-[1920px] grid-cols-12 gap-2 px-2">
      <aside
        class="sticky top-16 z-20 hidden h-[calc(100vh-225px)] flex-col gap-4 rounded-xl bg-[#131313] p-2 sm:col-span-4 sm:flex lg:col-span-3 2xl:col-span-2"
      >
        <section class="flex items-center justify-between px-2">
          <span class="font-semibold"> Your library </span>
          <PlusIcon class="h-6" />
        </section>
        <section
          class="flex flex-col items-start justify-center gap-2 rounded-xl bg-[#1d1d1d] p-4"
        >
          <h2 class="text-white">Create your first playlist</h2>
          <p class="text-sm">It's easy, we'll help you</p>
          <a
            href="#"
            class="mt-4 rounded-full bg-white px-4 py-1.5 text-sm font-semibold text-black transition duration-150 hover:scale-105 hover:bg-amber-50"
            >Create Playlist</a
          >
        </section>
        <section
          class="flex flex-col items-start justify-center gap-2 rounded-xl bg-[#1d1d1d] p-4"
        >
          <h2 class="text-white">Lets find some podcasts to follow</h2>
          <p class="text-sm">We'll keep you updated on new episodes</p>
          <a
            href="#"
            class="rounded-full bg-white px-4 py-1.5 text-sm font-semibold text-black transition duration-150 hover:scale-105 hover:bg-amber-50"
            >Browse podcasts</a
          >
        </section>
        <section class="my-auto">
          <ul class="flex flex-col gap-2">
            <li class="px-4 py-2 hover:underline">Legal</li>
            <li class="px-4 py-2 hover:underline">Safety & Privacy Center</li>
            <li class="px-4 py-2 hover:underline">Privacy Policy</li>
            <li class="px-4 py-2 hover:underline">Coockies</li>
            <li class="px-4 py-2 hover:underline">About Ads</li>
            <li class="px-4 py-2 hover:underline">Accessibility</li>
          </ul>
          <a
            href="#"
            class="m-4 flex w-fit items-center justify-between gap-1 rounded-full border border-[#aaaaaa] px-3 py-0 text-xs font-semibold text-white transition duration-150 hover:scale-105 hover:border-white"
          >
            <GlobeIcon class="h-8" />English</a
          >
        </section>
      </aside>

      <section
        class="col-span-12 overflow-y-auto rounded-xl bg-gradient-to-b from-[#191919] to-[#131313] sm:col-span-8 md:col-span-8 lg:col-span-9 2xl:col-span-10"
      >
        <div class="flex items-center justify-between p-2">
          <h1 class="text-xl text-white hover:underline">Trending songs</h1>
          <span class="text-xs font-semibold hover:underline">Show all</span>
        </div>
        <section class="flex items-center justify-between">
          <div
            class="group flex flex-col gap-2 rounded-xl p-4 hover:bg-[#2d2d2d]"
          >
            <div class="relative">
              <img src="/img/tranding-songs/1.png" class="rounded-xl" />
              <div
                class="absolute right-2 -bottom-2 opacity-0 transition-all duration-200 group-hover:bottom-2 group-hover:opacity-100 hover:scale-120"
              >
                <PlayLogo class="size-10" />
              </div>
            </div>
            <a href="#" class="font-semibold">Starboy (feat. Daft Punk)</a>
            <a href="#" class="text-xs">The Weekend</a>
          </div>
          <div
            class="group flex flex-col gap-2 rounded-xl p-4 hover:bg-[#2d2d2d]"
          >
            <div class="relative">
              <img src="/img/tranding-songs/2.png" class="rounded-xl" />
              <div
                class="absolute right-2 -bottom-2 opacity-0 transition-all duration-200 group-hover:bottom-2 group-hover:opacity-100 hover:scale-120"
              >
                <PlayLogo class="size-10" />
              </div>
            </div>
            <a href="#" class="font-semibold">Starboy (feat. Daft Punk)</a>
            <a href="#" class="text-xs">The Weekend</a>
          </div>
          <div
            class="group hidden flex-col gap-2 rounded-xl p-4 hover:bg-[#2d2d2d] sm:flex"
          >
            <div class="relative">
              <img src="/img/tranding-songs/3.png" class="rounded-xl" />
              <div
                class="absolute right-2 -bottom-2 opacity-0 transition-all duration-200 group-hover:bottom-2 group-hover:opacity-100 hover:scale-120"
              >
                <PlayLogo class="size-10" />
              </div>
            </div>
            <a href="#" class="font-semibold">Starboy (feat. Daft Punk)</a>
            <a href="#" class="text-xs">The Weekend</a>
          </div>
          <div
            class="group hidden flex-col gap-2 rounded-xl p-4 hover:bg-[#2d2d2d] md:flex"
          >
            <div class="relative">
              <img src="/img/tranding-songs/4.png" class="rounded-xl" />
              <div
                class="absolute right-2 -bottom-2 opacity-0 transition-all duration-200 group-hover:bottom-2 group-hover:opacity-100 hover:scale-120"
              >
                <PlayLogo class="size-10" />
              </div>
            </div>
            <a href="#" class="font-semibold">Starboy (feat. Daft Punk)</a>
            <a href="#" class="text-xs">The Weekend</a>
          </div>
          <div
            class="group hidden flex-col gap-2 rounded-xl p-4 hover:bg-[#2d2d2d] lg:flex"
          >
            <div class="relative">
              <img src="/img/tranding-songs/5.png" class="rounded-xl" />
              <div
                class="absolute right-2 -bottom-2 opacity-0 transition-all duration-200 group-hover:bottom-2 group-hover:opacity-100 hover:scale-120"
              >
                <PlayLogo class="size-10" />
              </div>
            </div>
            <a href="#" class="font-semibold">Starboy (feat. Daft Punk)</a>
            <a href="#" class="text-xs">The Weekend</a>
          </div>
          <div
            class="group hidden flex-col gap-2 rounded-xl p-4 hover:bg-[#2d2d2d] xl:flex"
          >
            <div class="relative">
              <img src="/img/tranding-songs/6.png" class="rounded-xl" />
              <div
                class="absolute right-2 -bottom-2 opacity-0 transition-all duration-200 group-hover:bottom-2 group-hover:opacity-100 hover:scale-120"
              >
                <PlayLogo class="size-10" />
              </div>
            </div>
            <a href="#" class="font-semibold">Starboy (feat. Daft Punk)</a>
            <a href="#" class="text-xs">The Weekend</a>
          </div>
          <div
            class="group hidden gap-2 rounded-xl p-4 hover:bg-[#2d2d2d] 2xl:flex 2xl:flex-col"
          >
            <div class="relative">
              <img src="/img/tranding-songs/7.png" class="rounded-xl" />
              <div
                class="group absolute right-2 -bottom-2 opacity-0 transition-all duration-200 group-hover:bottom-2 group-hover:opacity-100 hover:scale-120 hover:text-green-400"
              >
                <PlayLogo class="size-10 group-hover:text-blue-300" />
              </div>
            </div>

            <a href="#" class="font-semibold">Starboy (feat. Daft Punk)</a>
            <a href="#" class="text-xs">The Weekend</a>
          </div>
        </section>
        <div class="flex items-center justify-between p-2">
          <h1 class="text-xl text-white hover:underline">Popular artists</h1>
          <span class="text-xs font-semibold hover:underline">Show all</span>
        </div>
        <section class="flex items-center justify-between">
          <div
            class="group flex flex-col gap-2 rounded-xl p-4 hover:bg-[#2d2d2d]"
          >
            <div class="relative">
              <img src="/img/popular-artists/1.jpg" class="rounded-full" />
              <div
                class="group absolute right-2 -bottom-2 opacity-0 transition-all duration-200 group-hover:bottom-2 group-hover:opacity-100 hover:scale-120 hover:text-green-400"
              >
                <PlayLogo class="size-10 group-hover:text-blue-300" />
              </div>
            </div>
            <a href="#" class="font-semibold">Starboy (feat. Daft Punk)</a>
            <a href="#" class="text-xs">The Weekend</a>
          </div>
          <div
            class="group flex flex-col gap-2 rounded-xl p-4 hover:bg-[#2d2d2d]"
          >
            <div class="relative">
              <img src="/img/popular-artists/2.jpg" class="rounded-full" />
              <div
                class="group absolute right-2 -bottom-2 opacity-0 transition-all duration-200 group-hover:bottom-2 group-hover:opacity-100 hover:scale-120 hover:text-green-400"
              >
                <PlayLogo class="size-10 group-hover:text-blue-300" />
              </div>
            </div>
            <a href="#" class="font-semibold">Starboy (feat. Daft Punk)</a>
            <a href="#" class="text-xs">The Weekend</a>
          </div>
          <div
            class="group hidden flex-col gap-2 rounded-xl p-4 hover:bg-[#2d2d2d] sm:flex"
          >
            <div class="relative">
              <img src="/img/popular-artists/3.jpg" class="rounded-full" />
              <div
                class="group absolute right-2 -bottom-2 opacity-0 transition-all duration-200 group-hover:bottom-2 group-hover:opacity-100 hover:scale-120 hover:text-green-400"
              >
                <PlayLogo class="size-10 group-hover:text-blue-300" />
              </div>
            </div>
            <a href="#" class="font-semibold">Starboy (feat. Daft Punk)</a>
            <a href="#" class="text-xs">The Weekend</a>
          </div>
          <div
            class="group hidden flex-col gap-2 rounded-xl p-4 hover:bg-[#2d2d2d] lg:flex"
          >
            <div class="relative">
              <img src="/img/popular-artists/4.jpg" class="rounded-full" />
              <div
                class="group absolute right-2 -bottom-2 opacity-0 transition-all duration-200 group-hover:bottom-2 group-hover:opacity-100 hover:scale-120 hover:text-green-400"
              >
                <PlayLogo class="size-10 group-hover:text-blue-300" />
              </div>
            </div>
            <a href="#" class="font-semibold">Starboy (feat. Daft Punk)</a>
            <a href="#" class="text-xs">The Weekend</a>
          </div>
          <div
            class="group hidden flex-col gap-2 rounded-xl p-4 hover:bg-[#2d2d2d] xl:flex"
          >
            <div class="relative">
              <img src="/img/popular-artists/5.jpg" class="rounded-full" />
              <div
                class="group absolute right-2 -bottom-2 opacity-0 transition-all duration-200 group-hover:bottom-2 group-hover:opacity-100 hover:scale-120 hover:text-green-400"
              >
                <PlayLogo class="size-10 group-hover:text-blue-300" />
              </div>
            </div>
            <a href="#" class="font-semibold">Starboy (feat. Daft Punk)</a>
            <a href="#" class="text-xs">The Weekend</a>
          </div>
          <div
            class="group hidden flex-col gap-2 rounded-xl p-4 hover:bg-[#2d2d2d] 2xl:flex"
          >
            <div class="relative">
              <img src="/img/popular-artists/6.jpg" class="rounded-full" />
              <div
                class="group absolute right-2 -bottom-2 opacity-0 transition-all duration-200 group-hover:bottom-2 group-hover:opacity-100 hover:scale-120 hover:text-green-400"
              >
                <PlayLogo class="size-10 group-hover:text-blue-300" />
              </div>
            </div>
            <a href="#" class="font-semibold">Starboy (feat. Daft Punk)</a>
            <a href="#" class="text-xs">The Weekend</a>
          </div>
          <div
            class="group hidden flex-col gap-2 rounded-xl p-4 hover:bg-[#2d2d2d] 2xl:flex"
          >
            <div class="relative">
              <img src="/img/popular-artists/7.jpg" class="rounded-full" />
              <div
                class="group absolute right-2 -bottom-2 opacity-0 transition-all duration-200 group-hover:bottom-2 group-hover:opacity-100 hover:scale-120 hover:text-green-400"
              >
                <PlayLogo class="size-10 group-hover:text-blue-300" />
              </div>
            </div>
            <a href="#" class="font-semibold">Starboy (feat. Daft Punk)</a>
            <a href="#" class="text-xs">The Weekend</a>
          </div>
        </section>
        <div class="flex items-center justify-between p-2">
          <h1 class="text-xl text-white hover:underline">
            Popular albums and singers
          </h1>
          <span class="text-xs font-semibold hover:underline">Show all</span>
        </div>
        <section class="flex items-center justify-between">
          <div
            class="group flex flex-col gap-2 rounded-xl p-4 hover:bg-[#2d2d2d]"
          >
            <div class="relative">
              <img src="/img/albums-and-singers/1.png" class="rounded-xl" />
              <div
                class="group absolute right-2 -bottom-2 opacity-0 transition-all duration-200 group-hover:bottom-2 group-hover:opacity-100 hover:scale-120 hover:text-green-400"
              >
                <PlayLogo class="size-10 group-hover:text-blue-300" />
              </div>
            </div>
            <a href="#" class="font-semibold">Starboy (feat. Daft Punk)</a>
            <a href="#" class="text-xs">The Weekend</a>
          </div>
          <div
            class="group flex flex-col gap-2 rounded-xl p-4 hover:bg-[#2d2d2d]"
          >
            <div class="relative">
              <img src="/img/albums-and-singers/2.png" class="rounded-xl" />
              <div
                class="group absolute right-2 -bottom-2 opacity-0 transition-all duration-200 group-hover:bottom-2 group-hover:opacity-100 hover:scale-120 hover:text-green-400"
              >
                <PlayLogo class="size-10 group-hover:text-blue-300" />
              </div>
            </div>
            <a href="#" class="font-semibold">Starboy (feat. Daft Punk)</a>
            <a href="#" class="text-xs">The Weekend</a>
          </div>
          <div
            class="group hidden flex-col gap-2 rounded-xl p-4 hover:bg-[#2d2d2d] sm:flex"
          >
            <div class="relative">
              <img src="/img/albums-and-singers/3.png" class="rounded-xl" />
              <div
                class="group absolute right-2 -bottom-2 opacity-0 transition-all duration-200 group-hover:bottom-2 group-hover:opacity-100 hover:scale-120 hover:text-green-400"
              >
                <PlayLogo class="size-10 group-hover:text-blue-300" />
              </div>
            </div>
            <a href="#" class="font-semibold">Starboy (feat. Daft Punk)</a>
            <a href="#" class="text-xs">The Weekend</a>
          </div>
          <div
            class="group hidden flex-col gap-2 rounded-xl p-4 hover:bg-[#2d2d2d] lg:flex"
          >
            <div class="relative">
              <img src="/img/albums-and-singers/4.png" class="rounded-xl" />
              <div
                class="group absolute right-2 -bottom-2 opacity-0 transition-all duration-200 group-hover:bottom-2 group-hover:opacity-100 hover:scale-120 hover:text-green-400"
              >
                <PlayLogo class="size-10 group-hover:text-blue-300" />
              </div>
            </div>
            <a href="#" class="font-semibold">Starboy (feat. Daft Punk)</a>
            <a href="#" class="text-xs">The Weekend</a>
          </div>
          <div
            class="group hidden flex-col gap-2 rounded-xl p-4 hover:bg-[#2d2d2d] xl:flex"
          >
            <div class="relative">
              <img src="/img/albums-and-singers/5.png" class="rounded-xl" />
              <div
                class="group absolute right-2 -bottom-2 opacity-0 transition-all duration-200 group-hover:bottom-2 group-hover:opacity-100 hover:scale-120 hover:text-green-400"
              >
                <PlayLogo class="size-10 group-hover:text-blue-300" />
              </div>
            </div>
            <a href="#" class="font-semibold">Starboy (feat. Daft Punk)</a>
            <a href="#" class="text-xs">The Weekend</a>
          </div>
          <div
            class="group hidden flex-col gap-2 rounded-xl p-4 hover:bg-[#2d2d2d] 2xl:flex"
          >
            <div class="relative">
              <img src="/img/albums-and-singers/6.png" class="rounded-xl" />
              <div
                class="group absolute right-2 -bottom-2 opacity-0 transition-all duration-200 group-hover:bottom-2 group-hover:opacity-100 hover:scale-120 hover:text-green-400"
              >
                <PlayLogo class="size-10 group-hover:text-blue-300" />
              </div>
            </div>
            <a href="#" class="font-semibold">Starboy (feat. Daft Punk)</a>
            <a href="#" class="text-xs">The Weekend</a>
          </div>
          <div
            class="group hidden flex-col gap-2 rounded-xl p-4 hover:bg-[#2d2d2d] 2xl:flex"
          >
            <div class="relative">
              <img src="/img/albums-and-singers/7.png" class="rounded-xl" />
              <div
                class="group absolute right-2 -bottom-2 opacity-0 transition-all duration-200 group-hover:bottom-2 group-hover:opacity-100 hover:scale-120 hover:text-green-400"
              >
                <PlayLogo class="size-10 group-hover:text-blue-300" />
              </div>
            </div>
            <a href="#" class="font-semibold">Starboy (feat. Daft Punk)</a>
            <a href="#" class="text-xs">The Weekend</a>
          </div>
        </section>
        <div class="flex items-center justify-between p-2">
          <h1 class="text-xl text-white hover:underline">Popular radio</h1>
          <span class="text-xs font-semibold hover:underline">Show all</span>
        </div>
        <section class="flex items-center justify-evenly">
          <div
            class="group flex flex-col gap-2 rounded-xl p-4 hover:bg-[#2d2d2d]"
          >
            <div class="relative">
              <img src="/img/radio/1.png" class="rounded-xl" />
              <div
                class="group absolute right-2 -bottom-2 opacity-0 transition-all duration-200 group-hover:bottom-2 group-hover:opacity-100 hover:scale-120 hover:text-green-400"
              >
                <PlayLogo class="size-10 group-hover:text-blue-300" />
              </div>
            </div>
            <a href="#" class="font-semibold">Starboy (feat. Daft Punk)</a>
            <a href="#" class="text-xs">The Weekend</a>
          </div>
          <div
            class="group flex flex-col gap-2 rounded-xl p-4 hover:bg-[#2d2d2d]"
          >
            <div class="relative">
              <img src="/img/radio/2.png" class="rounded-xl" />
              <div
                class="group absolute right-2 -bottom-2 opacity-0 transition-all duration-200 group-hover:bottom-2 group-hover:opacity-100 hover:scale-120 hover:text-green-400"
              >
                <PlayLogo class="size-10 group-hover:text-blue-300" />
              </div>
            </div>
            <a href="#" class="font-semibold">Starboy (feat. Daft Punk)</a>
            <a href="#" class="text-xs">The Weekend</a>
          </div>
          <div
            class="group hidden flex-col gap-2 rounded-xl p-4 hover:bg-[#2d2d2d] sm:flex"
          >
            <div class="relative">
              <img src="/img/radio/3.png" class="rounded-xl" />
              <div
                class="group absolute right-2 -bottom-2 opacity-0 transition-all duration-200 group-hover:bottom-2 group-hover:opacity-100 hover:scale-120 hover:text-green-400"
              >
                <PlayLogo class="size-10 group-hover:text-blue-300" />
              </div>
            </div>
            <a href="#" class="font-semibold">Starboy (feat. Daft Punk)</a>
            <a href="#" class="text-xs">The Weekend</a>
          </div>
          <div
            class="group hidden flex-col gap-2 rounded-xl p-4 hover:bg-[#2d2d2d] md:flex"
          >
            <div class="relative">
              <img src="/img/radio/4.png" class="rounded-xl" />
              <div
                class="group absolute right-2 -bottom-2 opacity-0 transition-all duration-200 group-hover:bottom-2 group-hover:opacity-100 hover:scale-120 hover:text-green-400"
              >
                <PlayLogo class="size-10 group-hover:text-blue-300" />
              </div>
            </div>
            <a href="#" class="font-semibold">Starboy (feat. Daft Punk)</a>
            <a href="#" class="text-xs">The Weekend</a>
          </div>
          <div
            class="group hidden flex-col gap-2 rounded-xl p-4 hover:bg-[#2d2d2d] lg:flex"
          >
            <div class="relative">
              <img src="/img/radio/5.png" class="rounded-xl" />
              <div
                class="group absolute right-2 -bottom-2 opacity-0 transition-all duration-200 group-hover:bottom-2 group-hover:opacity-100 hover:scale-120 hover:text-green-400"
              >
                <PlayLogo class="size-10 group-hover:text-blue-300" />
              </div>
            </div>
            <a href="#" class="font-semibold">Starboy (feat. Daft Punk)</a>
            <a href="#" class="text-xs">The Weekend</a>
          </div>
          <div
            class="group hidden flex-col gap-2 rounded-xl p-4 hover:bg-[#2d2d2d] xl:flex"
          >
            <div class="relative">
              <img src="/img/radio/6.png" class="rounded-xl" />
              <div
                class="group absolute right-2 -bottom-2 opacity-0 transition-all duration-200 group-hover:bottom-2 group-hover:opacity-100 hover:scale-120 hover:text-green-400"
              >
                <PlayLogo class="size-10 group-hover:text-blue-300" />
              </div>
            </div>
            <a href="#" class="font-semibold">Starboy (feat. Daft Punk)</a>
            <a href="#" class="text-xs">The Weekend</a>
          </div>
          <div
            class="group hidden flex-col gap-2 rounded-xl p-4 hover:bg-[#2d2d2d] 2xl:flex"
          >
            <div class="relative">
              <img src="/img/radio/7.png" class="rounded-xl" />
              <div
                class="group absolute right-2 -bottom-2 opacity-0 transition-all duration-200 group-hover:bottom-2 group-hover:opacity-100 hover:scale-120 hover:text-green-400"
              >
                <PlayLogo class="size-10 group-hover:text-blue-300" />
              </div>
            </div>
            <a href="#" class="font-semibold">Starboy (feat. Daft Punk)</a>
            <a href="#" class="text-xs">The Weekend</a>
          </div>
        </section>
        <div class="flex items-center justify-between p-2">
          <h1 class="text-xl text-white hover:underline">Featured charts</h1>
          <span class="text-xs font-semibold hover:underline">Show all</span>
        </div>
        <section class="flex items-center">
          <div
            class="group flex flex-col gap-2 rounded-xl p-4 hover:bg-[#2d2d2d]"
          >
            <div class="relative">
              <img src="/img/featured-charts/1.png" class="rounded-xl" />
              <div
                class="group absolute right-2 -bottom-2 opacity-0 transition-all duration-200 group-hover:bottom-2 group-hover:opacity-100 hover:scale-120 hover:text-green-400"
              >
                <PlayLogo class="size-10 group-hover:text-blue-300" />
              </div>
            </div>
            <a href="#" class="font-semibold">Starboy (feat. Daft Punk)</a>
            <a href="#" class="text-xs">The Weekend</a>
          </div>
          <div
            class="group flex flex-col gap-2 rounded-xl p-4 hover:bg-[#2d2d2d]"
          >
            <div class="relative">
              <img src="/img/featured-charts/2.png" class="rounded-xl" />
              <div
                class="group absolute right-2 -bottom-2 opacity-0 transition-all duration-200 group-hover:bottom-2 group-hover:opacity-100 hover:scale-120 hover:text-green-400"
              >
                <PlayLogo class="size-10 group-hover:text-blue-300" />
              </div>
            </div>
            <a href="#" class="font-semibold">Starboy (feat. Daft Punk)</a>
            <a href="#" class="text-xs">The Weekend</a>
          </div>
          <div
            class="group hidden flex-col gap-2 rounded-xl p-4 hover:bg-[#2d2d2d] sm:flex"
          >
            <div class="relative">
              <img src="/img/featured-charts/3.png" class="rounded-xl" />
              <div
                class="group absolute right-2 -bottom-2 opacity-0 transition-all duration-200 group-hover:bottom-2 group-hover:opacity-100 hover:scale-120 hover:text-green-400"
              >
                <PlayLogo class="size-10 group-hover:text-blue-300" />
              </div>
            </div>
            <a href="#" class="font-semibold">Starboy (feat. Daft Punk)</a>
            <a href="#" class="text-xs">The Weekend</a>
          </div>
          <div
            class="group hidden flex-col gap-2 rounded-xl p-4 hover:bg-[#2d2d2d] md:flex"
          >
            <div class="relative">
              <img src="/img/featured-charts/4.png" class="rounded-xl" />
              <div
                class="group absolute right-2 -bottom-2 opacity-0 transition-all duration-200 group-hover:bottom-2 group-hover:opacity-100 hover:scale-120 hover:text-green-400"
              >
                <PlayLogo class="size-10 group-hover:text-blue-300" />
              </div>
            </div>
            <a href="#" class="font-semibold">Starboy (feat. Daft Punk)</a>
            <a href="#" class="text-xs">The Weekend</a>
          </div>
          <div
            class="group hidden flex-col gap-2 rounded-xl p-4 hover:bg-[#2d2d2d] lg:flex"
          >
            <div class="relative">
              <img src="/img/featured-charts/5.png" class="rounded-xl" />
              <div
                class="group absolute right-2 -bottom-2 opacity-0 transition-all duration-200 group-hover:bottom-2 group-hover:opacity-100 hover:scale-120 hover:text-green-400"
              >
                <PlayLogo class="size-10 group-hover:text-blue-300" />
              </div>
            </div>
            <a href="#" class="font-semibold">Starboy (feat. Daft Punk)</a>
            <a href="#" class="text-xs">The Weekend</a>
          </div>
          <div
            class="group hidden flex-col gap-2 rounded-xl p-4 hover:bg-[#2d2d2d] xl:flex"
          >
            <div class="relative">
              <img src="/img/featured-charts/6.png" class="rounded-xl" />
              <div
                class="group absolute right-2 -bottom-2 opacity-0 transition-all duration-200 group-hover:bottom-2 group-hover:opacity-100 hover:scale-120 hover:text-green-400"
              >
                <PlayLogo class="size-10 group-hover:text-blue-300" />
              </div>
            </div>
            <a href="#" class="font-semibold">Starboy (feat. Daft Punk)</a>
            <a href="#" class="text-xs">The Weekend</a>
          </div>
        </section>
        <footer class="w-full py-4 text-xs">
          <div class="flex flex-col justify-between gap-6 p-2 px-8 lg:flex-row">
            <ul class="flex flex-col items-center gap-2">
              <li class="font-semibold text-white hover:underline">Company</li>
              <li class="hover:underline">About</li>
              <li class="hover:underline">Jobs</li>
              <li class="hover:underline">For the Records</li>
            </ul>
            <ul class="flex flex-col items-center gap-2">
              <li class="font-semibold text-white hover:underline">
                Communities
              </li>
              <li class="hover:underline">For Artists</li>
              <li class="hover:underline">Developers</li>
              <li class="hover:underline">Advertising</li>
              <li class="hover:underline">Investors</li>
              <li class="hover:underline">Vendors</li>
            </ul>
            <ul class="flex flex-col items-center gap-2">
              <li class="font-semibold text-white hover:underline">
                Useful links
              </li>
              <li class="hover:underline">Support</li>
              <li class="hover:underline">Free Mobile</li>
              <li class="hover:underline">App</li>
            </ul>
            <ul class="flex flex-col items-center gap-2">
              <li class="font-semibold text-white">Spotify</li>
              <li class="hover:underline">Plans</li>
              <li class="hover:underline">Premium</li>
              <li class="hover:underline">Individual</li>
              <li class="hover:underline">Premium Duo</li>
              <li class="hover:underline">Premium Family</li>
              <li class="hover:underline">Premium Student</li>
              <li class="hover:underline">Spotify Free</li>
            </ul>
            <ul class="flex justify-center gap-2">
              <li
                class="h-fit rounded-full bg-gray-800 p-3 transition duration-150 hover:bg-gray-700"
              >
                <a href="#">
                  <InstagramLogo class="size-4" />
                </a>
              </li>
              <li
                class="h-fit rounded-full bg-gray-800 p-3 transition duration-150 hover:bg-gray-700"
              >
                <a href="#">
                  <TwitterLogo class="size-4" />
                </a>
              </li>
              <li
                class="h-fit rounded-full bg-gray-800 p-3 transition duration-150 hover:bg-gray-700"
              >
                <a href="#">
                  <FacebookLogo class="size-4" />
                </a>
              </li>
            </ul>
          </div>
        </footer>
      </section>
    </main>
    <section
      class="sticky bottom-0 z-20 flex h-36 w-full flex-col items-center justify-between gap-2 rounded-xl bg-gradient-to-r from-[#a6298b] to-[#4592f2] p-4 text-sm text-white lg:h-16 lg:flex-row"
      id="subscribe-bar"
    >
      <div>
        <h2>Prewiew of Spotify.</h2>
        <h2>
          Sign up to get unlimited songs and podcasts with occasional ads. No
          credit card needed.
        </h2>
      </div>
      <a
        href="#"
        class="rounded-full bg-white px-8 py-3 font-semibold text-black transition duration-150 hover:scale-105"
        >Sign up free</a
      >
    </section>
  </div>
</template>
