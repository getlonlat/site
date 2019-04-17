<template>
  <div class="home">
    <section class="hero is-light is-medium">
      <div class="hero-body">
        <div class="container">
          <h1 class="title">
            getLonLat
          </h1>
          <h2 class="subtitle">
            App utility to get coordinates from map.
          </h2>
        </div>
      </div>
    </section>

    <div class="container">
      <div class="section columns">
        <div
          class="column is-one-third"
          v-for="project in projects"
          v-bind:key="project.id"
        >
          <div class="card">
            <div class="card-header">
              <div class="card-header-title">
                {{ project.name }}
              </div>
            </div>
            <img :src="project.image" alt="" class="card-image" />
            <footer class="card-footer">
              <a :href="project.url" class="card-footer-item">
                <span class="icon"><i class="fas fa-external-link-alt"></i></span>
                <span>App</span>
              </a>
              <a :href="project.repository" class="card-footer-item">
                <span class="icon"><i class="fab fa-github"></i></span>
                <span>Repository</span>
              </a>
            </footer>
          </div>
        </div>
      </div>

    </div>

  </div>
</template>

<script>
export default {
  data() {
    return {
      projects: [
        {
          id: 1,
          name: "Angular",
          image: "img/angular.png",
          url: "https://angular.getlonlat.top",
          repository: "https://github.com/getlonlat/angular.git"
        },
        {
          id: 2,
          name: "Vue.js",
          image: "img/vuejs.png",
          url: "https://vuejs.getlonlat.top",
          repository: "https://github.com/getlonlat/vuejs.git"
        }
      ]
    };
  }
};
</script>
