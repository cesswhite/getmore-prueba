<template>
  <div class="app">
    <Hero />
    <History />
    <Product />
    <ActionImage />
    <Footer />
  </div>
</template>

<script setup>
useHead({
  title: 'Getmore | Test',
  viewport: 'width=device-width, initial-scale=1, maximum-scale=5',
  charset: 'utf-8',
  meta: [
    { name: 'description', content: 'This is a repo for testing purposes for getmore and cesswhite' }
  ],
  htmlAttrs: {
    lang: 'es'
  },
})
</script>

<style scoped>
.app {
  height: auto;
}
</style>