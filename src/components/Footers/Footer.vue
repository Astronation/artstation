<template>
  <footer
    class="pb-6"
    :class="[
      absolute ? 'absolute w-full bottom-0 bg-blueGray-800' : 'relative',
    ]"
  >
    <div class="container mx-auto px-4">
      <hr class="mb-6 border-b-1 border-blueGray-600" />
      <div
        class="flex flex-wrap items-center md:justify-between justify-center"
      >
        <div class="w-full md:w-4/12 px-4">
          <div
            class="text-sm text-blueGray-500 font-semibold py-1 text-center md:text-left"
          >
            Copyright © {{ date }}&nbsp;
            <a
              href="https://diamondapp.com/u/kanshi"
              class="text-white hover:text-blueGray-300 text-sm font-semibold py-1"
            >
              kanshi
            </a>
          </div>
        </div>
        <div class="w-full md:w-8/12 px-4">
          <ul class="flex flex-wrap list-none md:justify-end justify-center">
            <li>
              <a
                href="https://astronation.world/?ref=artstation-footer"
                class="text-white hover:text-blueGray-300 text-sm font-semibold block py-1 px-3"
              >
                Astronation
              </a>
            </li>
            <li>
              <a
                href="https://github.com/Astronation/artstation?ref=artstation-footer"
                class="text-white hover:text-blueGray-300 text-sm font-semibold block py-1 px-3"
              >
                GitHub
              </a>
            </li>
          </ul>
        </div>
      </div>
    </div>
  </footer>
</template>

<script>
export default {
  data() {
    return {
      date: new Date().getFullYear(),
    };
  },
  props: {
    absolute: {
      type: Boolean,
      default: false,
    },
  },
};
</script>
