<template>
  <section class="product-container">
    <div class="product-content">
      <div class="product-slide-info">
        <SliderInfo />
      </div>
      <div class="product-slide-products">
        <SliderProducts />
      </div>
    </div>
  </section>
</template>

<style scoped>
.product-container {
  height: auto;
  width: 100%;
}

.product-content {
  width: 100%;
  display: flex;
  flex-direction: column;
}

.product-slide-info {
  width: 100%;
}

.product-slide-products {
  width: 100%;
  height: auto;
}

@media screen and (min-width: 768px) {
  .product-content {
    width: 768px;
    margin: 0 auto;
  }
}

@media screen and (min-width: 1024px) {
  .product-content {
    width: 100%;
    flex-direction: row;
  }

  .product-slide-info {
    width: 50%;
  }

  .product-slide-products {
    width: 50%;
  }
}
</style>