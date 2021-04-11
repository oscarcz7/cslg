<template>
  <nav
    class="navbar is-transparent is-fixed-top p-4"
    role="navigation"
    aria-label="main navigation"
  >
    <div class="navbar-brand">
      <a class="navbar-item" href="/">
        <img src="@/assets/img/logo/logo.png" class="img-logo" />
      </a>
      <a
        role="button"
        class="navbar-burger burger"
        aria-label="menu"
        aria-expanded="false"
        data-target="navbarBasicExample"
      >
        <span aria-hidden="true"></span>
        <span aria-hidden="true"></span>
        <span aria-hidden="true"></span>
      </a>
    </div>
    <div id="navbar" class="navbar-menu">
      <div class="navbar-end">
        <router-link to="/" class="navbar-item">Inicio</router-link>
        <!-- Drop down menu for hs information about-->
        <div class="navbar-item has-dropdown is-hoverable">
          <router-link to="/" class="navbar-link"> Acerca de </router-link>

          <div class="navbar-dropdown">
            <a class="navbar-item"> ¿Quienes somos? </a>
            <a class="navbar-item"> Nuestra historia </a>
          </div>
        </div>
        <!-- Drop down menu for hs information sections directory-->
        <div class="navbar-item has-dropdown is-hoverable">
          <router-link to="/" class="navbar-link"> Direcciones </router-link>

          <div class="navbar-dropdown">
            <a class="navbar-item"> Académica </a>
            <a class="navbar-item"> Administrativa / Financiera </a>
            <a class="navbar-item"> Desarrollo Institucional </a>
            <a class="navbar-item"> Bienestar Estudiantil </a>
            <a class="navbar-item"> Pastoral </a>
          </div>
        </div>
        <!-- Drop down menu for hs information sections directory-->
        <div class="navbar-item has-dropdown is-hoverable">
          <router-link to="/" class="navbar-link"> Contacto </router-link>

          <div class="navbar-dropdown">
            <a class="navbar-item"> Contacto </a>
            <a class="navbar-item"> Buzon de Sugerencias </a>
          </div>
        </div>

        <div class="navbar-item">
          <div class="buttons">
            <a class="button is-dark">
              <strong>Log In</strong>
            </a>
          </div>
        </div>
      </div>
    </div>
  </nav>
</template>
<script>
export default {
  name: "Nav",
};
</script>
<style lang="scss" scoped>
nav {
  // margin-top: 25px;
  margin-bottom: 30px;
  a {
    font-weight: bold;
    color: #2c3e50;
    &.router-link-exact-active {
      color: #004a98;
    }
  }
}

.img-logo {
  max-width: 320px;
  max-height: 250px;
  margin: 0;
  padding: 0px;
}
</style>