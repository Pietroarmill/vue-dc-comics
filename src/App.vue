<template>
  <div id="app">
    <!-- Heaader -->
    <header>
      <AppHeader />
    </header>
    <!-- Heaader -->
    <!-- Main -->
    <main>
      <AppBanner />
      <AppProductsList />
      <RowBlue />
    </main>
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
import RowBlue from "./components/RowBlue.vue";
import AppBanner from "./components/AppBanner.vue";
import AppProductsList from "./components/AppProductsList.vue";

export default {
  name: "App",
  components: {
    AppHeader,
    AppFooter,
    RowBlue,
    AppBanner,
    AppProductsList,
  },
};
</script>
<style lang="scss">
@import "./style/common.scss";
@import "./style/variables.scss";
</style>
