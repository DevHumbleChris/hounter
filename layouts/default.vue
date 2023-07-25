<script setup>
useHead({
  htmlAttrs: {
    lang: 'en',
  },
  meta: [
    { property: 'og:title', content: `Hounter - House Hunter` },
    { name: 'description', content: 'Hounter - House Hunter built with Nuxt 3 and TailwindCSS.' },
    { property: 'og:description', content: 'Hounter - House Hunter built with Nuxt 3 and TailwindCSS.' },
    { property: 'og:url', content: 'https://hounter-ke.vercel.app/' },
    { name: 'twitter:title', content: 'Hounter - House Hunter' },
    { name: 'twitter:description', content: 'Hounter - House Hunter built with Nuxt 3 and TailwindCSS.' },
    { name: 'twitter:site', content: 'https://hounter-ke.vercel.app/' }
  ],
  title: `Hounter - House Hunter`,
})
</script>

<template>
  <main class="max-w-9xl font-lexend">
    <slot/>
  </main>
</template>
