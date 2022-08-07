<template>
  <button aria-label="primary-button" :class="color === 'white' ? 'color-white' : 'color-black'" class="primary-button">
    <slot />
    <svg class="arrow-icon" fill="none" stroke="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg">
      <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M17 8l4 4m0 0l-4 4m4-4H3"></path>
    </svg>
  </button>
</template>

<script setup lang="ts">
defineProps({
  color: String
})
</script>

<style scoped>
.primary-button {
  border-radius: 30px;
  font-size: .8rem;
  padding: 0.5em 1rem;
  height: 53px;
  background: none;
  appearance: none;
  width: 100%;
  font-weight: bold;
  text-transform: uppercase;
  display: flex;
  align-items: center;
  justify-content: center;
  gap: 1rem;
}

.color-white {
  border: 1px solid var(--white);
  color: var(--white);
}

.color-black {
  border: 1px solid var(--black);
  color: var(--black);
}

.arrow-icon {
  width: 25px;
}
</style>