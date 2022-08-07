<template>
  <a href=".#" class="link">
    <slot />
  </a>
</template>

<script setup lang="ts">

</script>

<style scoped>
.link {
  font-size: 1rem;
  font-weight: normal;
  line-height: normal;
  color: var(--white);
  letter-spacing: 1.5px;
  padding: 12px 0;
  position: relative;
  text-decoration: none;
}

.link:first-child {
  font-weight: bold;
}

.link:hover::before {
  content: '';
  position: absolute;
  width: 20px;
  height: 2px;
  background-color: #ffffff;
  bottom: 0;
  left: 0;
}
</style>