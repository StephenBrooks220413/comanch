<template>
  <div id="nav">
    <!-- Animated navbar-->
    <nav class="navbar navbar-expand-lg fixed-top navbar-scroll">
      <div class="container-fluid">
        <button
          class="navbar-toggler ps-0"
          type="button"
          data-mdb-toggle="collapse"
          data-mdb-target="#navbarExample01"
          aria-controls="navbarExample01"
          aria-expanded="false"
          aria-label="Toggle navigation"
        >
          <span
            class="
              navbar-toggler-icon
              d-flex
              justify-content-start
              align-items-center
            "
          >
            <i class="fas fa-bars"></i>
          </span>
        </button>
        <div class="collapse navbar-collapse" id="navbarExample01">
          <ul class="navbar-nav me-auto mb-2 mb-lg-0">
            <li class="nav-item active">
              <router-link class="nav-link active" to="/">Home</router-link>
            </li>
            <li class="nav-item">
              <router-link class="nav-link active" to="/about"
                >About</router-link
              >
            </li>
            <li class="nav-item">
              <router-link class="nav-link active" to="/contact"
                >Contact</router-link
              >
            </li>
          </ul>

          <ul class="navbar-nav flex-row">
            <!-- Icons -->
            <!-- Navbar dropdown -->
            <li class="nav-item dropdown">
              <a
                class="nav-link dropdown-toggle"
                href="#"
                id="navbarDropdown"
                role="button"
                data-mdb-toggle="dropdown"
                aria-expanded="false"
              >
                Dropdown
              </a>
              <!-- Dropdown menu -->
              <ul class="dropdown-menu" aria-labelledby="navbarDropdown">
                <li>
                  <router-link class="dropdown-item active" to="/services"
                    >Services</router-link
                  >
                </li>
                <li>
                  <router-link class="dropdown-item active" to="/services"
                    >Employment</router-link
                  >
                </li>
                <li><hr class="dropdown-divider" /></li>
                <li>
                  <router-link class="dropdown-item active" to="/services"
                    >Clients</router-link
                  >
                </li>
              </ul>
            </li>
            <li class="nav-item">
              <router-link class="nav-link active" to="/directory"
                >Directory</router-link
              >
            </li>
            <li class="nav-item">
              <a
                class="nav-link px-2"
                href="https://twitter.com/MDBootstrap"
                rel="nofollow"
                target="_blank"
              >
                <i class="fab fa-twitter"></i>
              </a>
            </li>
            <li class="nav-item">
              <a
                class="nav-link ps-2"
                href="https://github.com/mdbootstrap/mdb-ui-kit"
                rel="nofollow"
                target="_blank"
              >
                <i class="fab fa-facebook"></i>
              </a>
            </li>
          </ul>
        </div>
      </div>
    </nav>
    <!-- Animated navbar -->
  </div>
  <router-view />
</template>

<script>
import * as mdb from "mdb-ui-kit";

export default {
  mdb,
};
</script>

<style lang="scss">
@import "~mdb-ui-kit/css/mdb.min.css";

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
}

#nav {
  padding-bottom: 60px;

  a {
    font-weight: bold;
    color: #2c3e50;

    &.router-link-exact-active {
      color: #42b983;
    }
  }
}
</style>
