<template>
  <div class="single-product-container">
    <div class="single-index">
      {{ index }}
    </div>
    <img class="single-product-image" src="@/assets/products/group-10@3x.png" width="120" height="140" alt="">
  </div>
</template>

<script setup>
defineProps({
  index: Number
})
</script>


<style scoped>
.single-product-container {
  width: 288px;
  height: 100%;
  position: relative;
  background: var(--gray);
  scroll-snap-align: center;
  flex-shrink: 0;
  border-radius: 21px;
}

.single-product-image {
  width: 100%;
  height: 340px;
  object-fit: contain;
}

.single-index {
  width: 40px;
  height: 40px;
  position: absolute;
  top: 17px;
  left: 17px;
  border-radius: 50%;
  background: var(--green);
  display: flex;
  align-items: center;
  justify-content: center;
  font-size: 17px;
  font-weight: normal;
  line-height: 1.76;
  color: var(--white);
}
</style>