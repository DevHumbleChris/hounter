<script setup>
useHead({
  htmlAttrs: {
    lang: 'en',
  },
  meta: [
    { property: 'og:title', content: `Hounter` },
    { name: 'description', content: 'Hounter - House Hunter built with Nuxt 3 and TailwindCSS.' },
    { property: 'og:description', content: 'Hounter - House Hunter built with Nuxt 3 and TailwindCSS.' },
    { property: 'og:url', content: 'https://jadoo-ke.vercel.app/' },
    { name: 'twitter:title', content: 'Jadoo' },
    { name: 'twitter:description', content: 'Hounter - House Hunter built with Nuxt 3 and TailwindCSS.' },
    { name: 'twitter:site', content: 'https://jadoo-ke.vercel.app/' }
  ],
  title: `Jadoo`,
})
</script>

<template>
  <main class="max-w-8xl">
    <slot/>
  </main>
</template>
