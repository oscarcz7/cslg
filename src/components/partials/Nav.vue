<template>
  <nav
    class="navbar is-transparent  p-4"
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
        <router-link to="/about" class="navbar-item"> El Gonzaga </router-link>
        
        <!-- Drop down menu for hs information sections directory-->
        <div class="navbar-item has-dropdown is-hoverable">
          <router-link to="/" class="navbar-link"> Direcciones </router-link>

          <div class="navbar-dropdown">
            <router-link to="/academica" class="navbar-item"> Académica </router-link>
            <router-link to="/financiera" class="navbar-item"> Administrativa / Financiera </router-link>
            <router-link to="/desarrollo-institucional" class="navbar-item"> Desarrollo Institucional </router-link>
            <router-link to="/bienestar" class="navbar-item"> Bienestar Estudiantil </router-link>
            <router-link to="/pastoral" class="navbar-item"> Pastoral </router-link>
          </div>
        </div>
        <!-- Drop down menu for hs information sections directory-->
        <div class="navbar-item has-dropdown is-hoverable">
          <router-link to="/" class="navbar-link"> Contacto </router-link>

          <div class="navbar-dropdown">
            <router-link to="/contacto" class="navbar-item"> Contacto </router-link>
            <router-link to="/buzon" class="navbar-item"> Buzon de Sugerencias </router-link>
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