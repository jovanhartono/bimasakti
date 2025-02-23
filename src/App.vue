<script setup lang="ts">
import { RouterLink, RouterView } from 'vue-router'
</script>

<template>
  <header class="sticky top-0 z-50 h-18 bg-white/50 backdrop-blur">
    <nav class="mx-auto flex h-full max-w-screen-lg items-center p-4">
      <RouterLink to="/">
        <img
          draggable="false"
          src="https://xnxk060v5p.ufs.sh/f/D0ooyPBt8scPK0IVi91HBhyQbeCRGNZt0UP57daFTruIXJpD"
          alt="bimasakti wordmark"
          class="h-6"
        />
      </RouterLink>
      <ul class="ml-auto flex items-center gap-x-4 font-medium">
        <a href="#about" class="ml-auto">About Us</a>
        <a href="#contact" class="ml-auto rounded-md bg-blue-900 px-3 py-2 text-white"
          >Contact Us</a
        >
      </ul>
    </nav>
  </header>

  <RouterView />

  <footer class="flex h-20 items-center border-t bg-gradient-to-br px-0 text-blue-950">
    <div class="container tracking-wide max-sm:text-center max-sm:text-sm max-sm:text-balance">
      &copy; 2025 PT Bimasakti Nawasena Sejahtera. All rights reserved.
    </div>
  </footer>
</template>
