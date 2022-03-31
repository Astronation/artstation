<template>
  <nav
    class="top-0 fixed z-50 w-full flex flex-wrap items-center justify-between px-2 py-3 navbar-expand-lg bg-white shadow"
  >
    <div
      class="container px-4 mx-auto flex flex-wrap items-center justify-between"
    >
      <div
        class="w-full relative flex justify-between lg:w-auto lg:static lg:block lg:justify-start"
      >
        <router-link to="/">
          <a
            class="text-blueGray-700 text-sm font-bold leading-relaxed inline-block mr-4 py-2 whitespace-nowrap uppercase"
            href="#"
          >
            ArtStation
          </a>
        </router-link>
        <button
          class="cursor-pointer text-xl leading-none px-3 py-1 border border-solid border-transparent rounded bg-transparent block lg:hidden outline-none focus:outline-none"
          type="button"
          v-on:click="setNavbarOpen"
        >
          <i class="fas fa-bars"></i>
        </button>
      </div>
      <div
        class="lg:flex flex-grow items-center"
        :class="[navbarOpen ? 'block' : 'hidden']"
        id="example-navbar-warning"
      >
        <ul class="flex flex-col lg:flex-row list-none lg:ml-auto">
          
          <li class="flex items-center">
            <a
              class="hover:text-blueGray-500 text-blueGray-700 px-3 py-2 flex items-center text-xs uppercase font-bold"
              href="https://www.facebook.com/sharer/sharer.php?u=https%3A%2F%2Fastronation.world%2Fstations%2Fartstation"
              target="_blank"
            >
              <i class="text-blueGray-400 fab fa-facebook text-lg leading-lg" />
              <span class="lg:hidden inline-block ml-2">Share</span>
            </a>
          </li>

          <li class="flex items-center">
            <a
              class="hover:text-blueGray-500 text-blueGray-700 px-3 py-2 flex items-center text-xs uppercase font-bold"
              href="https://twitter.com/intent/tweet?url=https%3A%2F%2Fastronation.world%2Fstations%2Fartstation&text=Check%20the%20first%20PSC%20in%20the%20metaverse!%20"
              target="_blank"
            >
              <i class="text-blueGray-400 fab fa-twitter text-lg leading-lg" />
              <span class="lg:hidden inline-block ml-2">Tweet</span>
            </a>
          </li>

          <li class="flex items-center">
            <a
              class="hover:text-blueGray-500 text-blueGray-700 px-3 py-2 flex items-center text-xs uppercase font-bold"
              href="https://github.com/Astronation/artstation?ref=index-navbar"
              target="_blank"
            >
              <i class="text-blueGray-400 fab fa-github text-lg leading-lg" />
              <span class="lg:hidden inline-block ml-2">Star</span>
            </a>
          </li>
          <li class="flex items-center">
            <a
              class="hover:text-blueGray-500 text-blueGray-700 px-3 py-2 flex items-center text-xs uppercase font-bold"
              href="https://discord.gg/NJQeACHgjY"
              target="_blank"
            >
              <i class="text-blueGray-400 fab fa-discord text-lg leading-lg" />
              <span class="lg:hidden inline-block ml-2">Discord</span>
            </a>
          </li>
          <!--
          <li class="flex items-center">
            <a
              class="hover:text-blueGray-500 text-blueGray-700 px-3 py-2 flex items-center text-xs uppercase font-bold"
              href="#whitepaper-url"
            >
              <i
                class="text-blueGray-400 far fa-file-alt text-lg leading-lg mr-2"
              />
              Whitepaper
            </a>
          </li>
        -->
        </ul>
      </div>
    </div>
  </nav>
</template>

<script>

export default {
  data() {
    return {
      navbarOpen: false,
    };
  },
  methods: {
    setNavbarOpen: function () {
      this.navbarOpen = !this.navbarOpen;
    },
  },
  components: {
    
  },
};
</script>
