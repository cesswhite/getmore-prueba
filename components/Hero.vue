<template>
  <div class="hero-container">
    <SideBar />
    <div class="hero-content">
      <Header />
      <div class="cta-container">
        <div class="text-container">
          <h1 class="text-title">Las mejores raquetas para jugar <span class="text-green">Tennis</span></h1>
          <div class="button-container">
            <Button color="white">
              Acerca de Nosotros
            </Button>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped>
.hero-container {
  background: url("@/assets/hero/group@3x.jpg") no-repeat center center;
  background-size: cover;
  width: 100%;
  height: 100vh;
  display: flex;
}

.hero-content {
  width: 100%;
  height: 100%;
}

.cta-container {
  width: 100%;
  height: 100%;
  display: flex;
  align-items: center;
  justify-content: left;
  padding: 0 20px;
}

.text-container {
  width: 100%;
  display: flex;
  flex-direction: column;
  gap: 2rem;
}

.text-title {
  font-size: 36px;
  font-weight: normal;
  line-height: 1.28;
  color: var(--white);
}

.text-green {
  color: var(--green);
  font-weight: bold;
}

.button-container {
  max-width: 75%;
}

@media screen and (min-width: 768px) {

  .button-container {
    width: 50%;
  }

  .text-title {
    font-size: 53px;
  }


}

@media screen and (min-width: 1024px) {
  .cta-container {
    padding: 0 67px;
  }

  .text-container {
    width: 40%;
  }

  .button-container {
    width: 50%;
  }
}
</style>