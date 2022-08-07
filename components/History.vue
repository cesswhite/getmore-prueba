<template>
  <section class="history-container">
    <div class="info-container">
      <div class="text-helper">
        TENNIS
      </div>
      <div class="description-container">
        <h2 class="info-title">
          Raquetas.Accesorios.Pelotas.
        </h2>
        <p class="info-description">
          Conoce nuestras raquetas y aprende a jugar Tennis cómo un profesional.
        </p>

      </div>
      <div class="button-container">
        <Button>
          Historia
        </Button>
      </div>
    </div>
  </section>
</template>

<script setup>

</script>

<style scoped>
.history-container {
  height: 400px;
  width: 100%;
  background: var(--gray);
  display: flex;
  align-items: center;
}

.info-container {
  width: 100%;
  padding: 0 20px;
  display: flex;
  flex-direction: column;
}

.description-container {
  display: flex;
  flex-direction: column;
  gap: 1rem;
}

.text-helper {
  color: var(--green);
  font-size: .9rem;
  font-weight: bold;
}

.info-title {
  font-size: 2.25rem;
  color: var(--black);
  font-weight: normal;
  line-height: 1.14;
  hyphens: auto;
  width: 100%;
}

.button-container {
  width: 75%;
  margin-top: 1rem;
}

.info-description {
  font-size: 1.1rem;
  font-weight: normal;
  color: var(--gray-secondary);
}

@media screen and (min-width: 768px) {
  .button-container {
    width: 50%;
  }
}

@media screen and (min-width: 1024px) {
  .info-container {
    width: 768px;
    padding: 0;
    margin: 0 auto;
  }
}

@media screen and (min-width: 1280px) {
  .info-container {
    width: 1024px;
    justify-content: center;
    gap: 2rem;
  }

  .info-container {
    flex-direction: row;
  }

  .info-title {
    width: 65%;
  }

  .info-description {
    width: 75%;
  }

  .button-container {
    width: 20%;
    margin-top: 0;
    display: flex;
    align-items: flex-end;
  }

  .text-helper {
    padding-top: .5rem;
  }
}
</style>