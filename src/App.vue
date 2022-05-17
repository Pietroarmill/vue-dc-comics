<template>
  <div id="app">
    <!-- Heaader -->
    <header>
      <AppHeader />
    </header>
    <!-- Heaader -->
    <!-- Main -->
    <main></main>
    <!-- Main -->
    <!-- Footer -->
    <footer></footer>
    <!-- Footer -->
  </div>
</template>
<script>
import AppHeader from "./components/AppHeader.vue";
export default {
  name: "App",
  components: {
    AppHeader,
  },
};
</script>
<style lang="scss"></style>
