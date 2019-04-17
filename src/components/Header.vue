<template>
  <nav class="navbar is-light" role="navigation" aria-label="main navigation">
    <div class="container">
      <div class="navbar-brand">
        <a class="navbar-item" href="">
          <img
            src="@/assets/img/target.png"
            style="margin-right: 5px;"
            alt=""
          />
          <router-link to="/" class="is-size-4" tag="span">
            getLonLat
          </router-link>
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

      <div id="navbarBasicExample" class="navbar-menu">
        <div class="navbar-end">
          <div class="navbar-item">
            <div class="buttons">
              <router-link to="/about" class="button is-light is-inverted">
                About
              </router-link>
            </div>
          </div>
        </div>
      </div>
    </div>
  </nav>
</template>
