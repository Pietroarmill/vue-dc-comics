<template>
  <div class="banner__bg"></div>
</template>

<script>
export default {
  name: "AppBanner",
};
</script>

<style lang="scss" scoped>
@import "../style/common.scss";
@import "../style/variables.scss";

.banner__bg {
  height: 300px;
  background-image: url(../assets/img/jumbotron.jpg);
  background-size: cover;
}
</style>
