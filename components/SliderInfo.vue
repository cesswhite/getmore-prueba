<template>
  <div class="slider-info-container">
    <img class="slider-img" width="375" height="468" src="@/assets/products/ball-color-court-1405355@3x.png" alt="">
    <div class="slider-info">
      <h2 class="slider-title">
        Nuestras <br>
        <b>Raquetas</b>
      </h2>
      <p class="slider-description">
        Conoce nuestras raquetas y aprende a jugar Tennis cómo un profesional.
      </p>
      <div class="slider-bullet-container">
        <span class="slider-bullet active" />
        <span class="slider-bullet" />
        <span class="slider-bullet" />
        <span class="slider-bullet" />
      </div>
      <div class="button-container">
        <button aria-label="button-icon" class="slider-button inactive">
          <svg class="arrow-icon" viewBox="0 0 15 15" xmlns="http://www.w3.org/2000/svg">
            <path d="M9 4L9 11L4.5 7.5L9 4Z" />
          </svg>
        </button>
        <button aria-label="button-icon" class="slider-button active">
          <svg class="arrow-icon" viewBox="0 0 15 15" xmlns="http://www.w3.org/2000/svg">
            <path d="M6 11L6 4L10.5 7.5L6 11Z" />
          </svg>
        </button>
      </div>
    </div>
  </div>
</template>

<style scoped>
.slider-info-container {
  height: 375px;
  position: relative;
}

.slider-info {
  position: absolute;
  width: 100%;
  padding: 0 20px;
  margin: 0;
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
}

.slider-img {
  width: 100%;
  height: 100%;
  object-fit: cover;
  object-position: center;
}

.slider-title {
  font-size: 50px;
  font-weight: normal;
  line-height: 1.28;
  color: var(--white);
}

.slider-description {
  font-size: 18px;
  font-weight: normal;
  line-height: 1.67;
  margin-top: 1rem;
  color: var(--white);
}

.slider-bullet-container {
  display: flex;
  gap: 1rem;
  margin-top: 1rem;
}

.slider-bullet {
  border-radius: 50%;
  width: 8px;
  height: 8px;
  display: inline;
  background: var(--bullet);
}

.slider-bullet.active {
  background: var(--green);
}

.button-container {
  display: flex;
  gap: 1rem;
  margin-top: 1rem;
}

.slider-button {
  border-radius: 50%;
  width: 54px;
  height: 54px;
  display: flex;
  align-items: center;
  justify-content: center;
  border: none;
}

.slider-button {
  background: none;
  border: 1px solid var(--white);
}

/* .slider-button.active {
  background-color: var(--green);
  box-shadow: 0px 4px 12px 0px rgba(0, 0, 0, 0.4);
} */

.slider-button:hover {
  cursor: pointer;
  background-color: var(--green);
  box-shadow: 0px 4px 12px 0px rgba(0, 0, 0, 0.4);
}

.arrow-icon {
  fill: var(--white);
  width: 32px;
  height: 32px;
}

@media screen and (min-width: 1024px) {
  .slider-info-container {
    display: flex;
    justify-content: flex-end;
  }
}

@media screen and (min-width: 1280px) {
  .slider-info {
    width: 50%;
    left: 0;
    right: 10%;
    transform: translate(90%, -50%);
  }
}
</style>