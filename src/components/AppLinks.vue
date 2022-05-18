<template>
  <ul class="links-list">
    <li class="link">
      <a href="">{{ linkObj.text }}</a>
    </li>
  </ul>
</template>

<script>
export default {
  name: "AppLinks",
  props: {
    linkObj: Object,
  },
};
</script>

<style lang="scss" scoped>
@import "../style/common.scss";
@import "../style/variables.scss";

.links-list .link {
  a {
    font-size: 0.8rem;
  }
}
</style>
