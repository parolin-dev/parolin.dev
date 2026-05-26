<script setup lang="ts">
import SmilingEmoji from "../assets/emojis/smiling.png";
import LinkedInButton from "./common/LinkedInButton.vue";
import GitHubButton from "./common/GitHubButton.vue";
import FullstackDevCard from "./welcome/FullstackDevCard.vue";
</script>

<template>
  <section class="flex w-full flex-col items-center px-6 md:px-8 lg:max-w-6xl">
    <div class="mt-6 mb-16 flex flex-col items-center justify-center">
      <img :src="SmilingEmoji" class="mb-4 h-32" alt="Matteo Parolin emoji" />

      <h1 class="text-center text-2xl font-bold tracking-tighter text-white">
        Matteo Parolin
      </h1>
      <p class="text-center text-sm font-medium tracking-tight text-white/75">
        Freelance web app developer
      </p>

      <div class="mt-2 flex gap-2">
        <LinkedInButton />
        <GitHubButton />
      </div>
    </div>

    <FullstackDevCard />
  </section>
</template>
