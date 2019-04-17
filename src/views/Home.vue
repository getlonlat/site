<template>
  <div class="home">
    <div class="columns">
      <div
        class="column is-half"
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
