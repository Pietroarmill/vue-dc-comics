<template>
  <header class="header">
    <div class="container">
      <div class="header__logo">
        <img src="../assets/img/dc-logo.png" alt="" />
      </div>
      <nav>
        <ul class="header__menu">
          <li
            v-for="(item, index) in links"
            :key="index"
            :class="{ active: item.value === true }"
          >
            <a href="">{{ item.text.toUpperCase() }}</a>
          </li>
        </ul>
      </nav>
    </div>
  </header>
</template>

<script>
export default {
  name: "AppHeader",
  data() {
    return {
      links: [
        {
          url: "",
          text: "characters",
          value: false,
        },
        {
          url: "",
          text: "comics",
          value: true,
        },
        {
          url: "",
          text: "movies",
          value: false,
        },
        {
          url: "",
          text: "tv",
          value: false,
        },
        {
          url: "",
          text: "games",
          value: false,
        },
        {
          url: "",
          text: "collectibles",
          value: false,
        },
        {
          url: "",
          text: "videos",
          value: false,
        },
        {
          url: "",
          text: "fans",
          value: false,
        },
        {
          url: "",
          text: "news",
          value: false,
        },
        {
          url: "",
          text: "shop",
          value: false,
        },
      ],
    };
  },
};
</script>
<style lang="scss">
@import "../style/common.scss";
@import "../style/variables.scss";

.header {
  .container {
    display: flex;
    justify-content: space-between;
    align-items: center;
  }
  &__logo {
    width: 80px;
  }
  &__menu {
    display: flex;
    li {
      line-height: 105px;
      border-bottom: 3px solid transparent;
      margin: 0 1rem;
      font-size: 0.8rem;
      font-weight: 700;
      &.active {
        border-bottom: 5px solid $brand-primary-color;
      }
      a {
        color: black;
      }
    }
  }
}
</style>
