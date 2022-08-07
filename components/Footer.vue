<template>
  <footer class="footer-container">
    <div class="footer-content">
      <div class="footer-info-container">
        <nav class="nav-links">
          <template v-for="link in links">
            <a class="footer-link">
              {{ link }}
            </a>
          </template>
        </nav>
        <div class="footer-icons-container">
          <button class="button-network">
            <img src="@/assets/icons/linkedin.svg" width="31" height="31" class="" alt="">
          </button>
          <button class="button-network">
            <img src="@/assets/icons/vimeo.svg" width="31" height="31" class="" alt="">
          </button>
          <button class="button-network">
            <img src="@/assets/icons/instagram.svg" width="31" height="31" class="" alt="">
          </button>
          <button class="button-network">
            <img src="@/assets/icons/twitter.svg" width="31" height="31" class="" alt="">
          </button>
          <button class="button-network">
            <img src="@/assets/icons/facebook.svg" width="31" height="31" class="" alt="">
          </button>
        </div>
      </div>
      <div class="logo-container">
        <img width="12" height="12" class="logo-img" src="/fill-2.svg" alt="" />
      </div>
    </div>
  </footer>
</template>
<script setup>
const links = ['Inicio', 'Acerca de nosotros', 'Historia', 'Contacto']
</script>
<style scoped>
.footer-container {
  width: 100%;
  height: 203px;
  background: var(--green);
  padding: 2rem 1rem;
  display: flex;
  justify-content: center;
  align-items: center;
}

.footer-content {
  display: flex;
  flex-direction: column;
}

.footer-info-container {
  width: 100%;
}

.nav-links {
  display: flex;
  justify-content: space-between;
  gap: 1rem;
}

.footer-link {
  font-size: 13px;
  color: var(--dark-blue);
  line-height: normal;
}

.footer-icons-container {
  width: 100%;
  display: flex;
  gap: 1rem;
  justify-content: space-evenly;
  margin-top: 1rem;
}

.button-network {
  width: 32px;
  height: 32px;
  border: 1px solid var(--white);
  border-radius: 50%;
  display: flex;
  align-items: center;
  justify-content: center;
  background: none;
}

.logo-container {
  width: 100%;
  margin-top: 1rem;
  display: flex;
  align-items: center;
}

.logo-img {
  margin: 0 auto;
  width: 32px;
  height: 32px;
}

@media screen and (min-width: 768px) {
  .footer-content {
    flex-direction: row;
    justify-content: space-between;
  }

  .footer-info-container {
    width: 50%;
  }

  .logo-container {
    width: auto;
    margin-top: 0;
  }

  .footer-icons-container {
    width: 100%;
    display: flex;
    gap: 1rem;
    justify-content: flex-start;
    margin-top: 1rem;
  }

  .nav-links {
    justify-content: flex-start;
  }
}

@media screen and (min-width: 1280px) {
  .footer-content {
    width: 1280px;
    margin: 0 auto;
    padding: 0 20px;
  }
}
</style>