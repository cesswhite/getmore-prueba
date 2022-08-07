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
  title: 'Eco Development Studios',
  viewport: 'width=device-width, initial-scale=1, maximum-scale=5',
  charset: 'utf-8',
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