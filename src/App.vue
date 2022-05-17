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
    <footer>
      <AppFooter />
    </footer>
    <!-- Footer -->
  </div>
</template>
<script>
import AppHeader from "./components/AppHeader.vue";
import AppFooter from "./components/AppFooter.vue";

export default {
  name: "App",
  components: {
    AppHeader,
    AppFooter,
  },
};
</script>
<style lang="scss"></style>
