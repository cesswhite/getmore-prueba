<template>
  <div class="slider-products-container">
    <template v-for="n in 10" :key="n">
      <SingleProduct :index="n" />
    </template>
  </div>
</template>

<script setup>

</script>

<style scoped>
.slider-products-container {
  height: auto;
  position: relative;
  width: 100%;
  display: flex;
  gap: 1.5rem;
  scroll-snap-type: x mandatory;
  overflow-x: auto;
  padding: 20px 20px 10px 20px;
}
</style>