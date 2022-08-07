<template>
  <header class="header-container align-items">
    <img width="37" height="37" class="logo-img" src="@/assets/fill-2.svg" alt="" />
    <nav class="align-items nav-container">
      <template v-for="link in links">
        <Link>
        {{ link }}
        </Link>
      </template>
    </nav>
    <div class="align-items nav-language">
      <Link>
      ES
      </Link>
      <Link>
      EN
      </Link>

      <svg class="menu-icon" fill="none" stroke="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg">
        <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 6h16M4 12h16M4 18h16"></path>
      </svg>

    </div>
  </header>
</template>

<script setup>
const links = ['Inicio', 'Acerca de nosotros', 'Historia', 'Contacto']
</script>

<style scoped>
.header-container {
  position: absolute;
  width: 100%;
  top: 40px;
  left: 0;
  justify-content: space-between;
  padding: 0 20px;
}

.align-items {
  display: flex;
  align-items: center;
  gap: 1rem;
}

.nav-container {
  display: none;
}

.nav-container>a:first-child:before {
  content: '';
  position: absolute;
  width: 20px;
  height: 2px;
  background-color: #ffffff;
  bottom: 0;
  left: 0;
}

.menu-icon {
  width: 28px;
  height: 28px;
  color: #ffffff;
}

.logo-img {
  display: inline;
}

.nav-language {}

@media screen and (min-width: 1024px) {
  .nav-container {
    display: flex;
  }

  .menu-icon {
    display: none;
  }

  .logo-img {
    display: none;
  }

  .align-items {
    gap: 2rem;
  }

  .header-container {
    position: absolute;
    padding: 0 160px;
  }
}
</style>