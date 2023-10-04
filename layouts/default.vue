<template>
  <header>
    <nav class="flex items-center gap-8 justify-between">
      <div class="flex items-center gap-4">
        <NuxtImg src="/profil.jpg" class="rounded-full w-24"/>
        <h2>Développeur Frontend</h2>
      </div>
      <div>
        <nuxt-link to="/">Github</nuxt-link>
        <nuxt-link to="/">Contact</nuxt-link>
      </div>
    </nav>
  </header>
  <slot />
</template>
<script setup lang="ts">
</script>