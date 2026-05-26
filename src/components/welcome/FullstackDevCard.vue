<script setup lang="ts">
import Globe from "./LightedGlobe.vue";
import Laravel from "../../assets/technologies/laravel.svg";
import VueJS from "../../assets/technologies/vuejs.svg";
import Tailwind from "../../assets/technologies/tailwind.svg";
</script>

<template>
  <div
    class="flex max-w-[50em] flex-col items-center justify-center gap-8 md:flex-row md:px-8"
  >
    <div class="text-white">
      <h2 class="text-center font-medium">Web app development</h2>
      <p class="text-center text-sm text-white/75">
        Web development services delivering unique front-end experiences
        combined with robust back-end architecture, all tailored to boost user
        engagement and support business objectives.
      </p>
    </div>

    <div class="relative flex h-52 w-full justify-center overflow-hidden">
      <div class="absolute -bottom-18 flex w-full justify-center">
        <Globe class="h-70 rotate-12" aria-hidden="true" />
      </div>

      <div
        class="absolute bottom-1 z-20 flex items-center gap-1 font-mono text-xs tracking-tight text-white/60 uppercase"
      >
        <img :src="Laravel" class="mb-1 h-3 grayscale" aria-hidden="true" />
        Laravel <span aria-hidden="true">+</span>
        <img :src="VueJS" class="mb-1 h-3 grayscale" aria-hidden="true" />
        Vue.js <span aria-hidden="true">+</span>
        <img :src="Tailwind" class="mb-1 h-4 grayscale" aria-hidden="true" />
        Tailwind
      </div>

      <div
        class="absolute bottom-0 left-0 z-10 h-20 w-full bg-gradient-to-b from-transparent to-neutral-950"
      ></div>
    </div>
  </div>
</template>
