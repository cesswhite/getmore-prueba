<template>
  <div class="sidebar-container">
    <img width="37" height="37" class="logo-img" src="@/assets/fill-2.svg" alt="">
  </div>
</template>


<style scoped>
.sidebar-container {
  width: 205px;
  height: 100%;
  border-right: 1px solid var(--white);
  display: none;
}

.logo-img {
  margin: 0 auto;
  margin-top: 25px;
}

@media screen and (min-width: 1024px) {
  .sidebar-container {
    width: 105px;
    display: flex;
  }
}
</style>