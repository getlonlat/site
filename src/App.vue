<template>
  <div id="app">
    <app-header></app-header>
    <hr />
    <div class="container">
      <router-view />
    </div>
  </div>
</template>

<script>
import Header from "@/components/Header.vue";

export default {
  components: {
    appHeader: Header
  }
};
</script>

<style lang="scss">
@import "~bulma/bulma";
</style>
