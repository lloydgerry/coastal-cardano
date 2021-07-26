<template>
  <div class="app">
    <NavBar />
    <div class="body">
      <router-view />
    </div>
  </div>
</template>

<script>
import NavBar from "@/views/components/NavBar.vue";

export default {
  components: {
    NavBar,
  }
}
</script>

<style>
.app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  /* move page down height of NavBar */
  margin-top: 60px;

}

.body {
  width: 100vw;
  min-height: 100vh;
}
</style>
