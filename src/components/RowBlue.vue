<template>
  <div class="row__blue">
    <div class="container">
      <ul>
        <li v-for="(item, index) in comics" :key="index">
          <div class="row__blue__image">
            <img :src="require(`../assets/img/${item.image}.png`)" alt="" />
          </div>
          <div>{{ item.text.toUpperCase() }}</div>
        </li>
      </ul>
    </div>
  </div>
</template>

<script>
export default {
  name: "RowBlue",
  data() {
    return {
      comics: [
        {
          url: "",
          text: "digital comics",
          image: "buy-comics-digital-comics",
        },
        {
          url: "",
          text: "dc merchandise",
          image: "buy-comics-merchandise",
        },
        {
          url: "",
          text: "subscription",
          image: "buy-comics-subscriptions",
        },
        {
          url: "",
          text: "comic shop locator",
          image: "buy-comics-shop-locator",
        },
        {
          url: "",
          text: "dc power visa",
          image: "buy-comics-shop-locator",
        },
      ],
    };
  },
};
</script>

<style lang="scss">
@import "../style/common.scss";
@import "../style/variables.scss";

.row__blue {
  background-color: $brand-primary-color;
  height: 170px;
  display: flex;
  align-items: center;
  ul {
    display: flex;
    justify-content: space-evenly;
    li {
      display: flex;
      align-items: center;
      font-size: 0.8rem;
      font-weight: 600;
      color: white;
    }
  }
  &__image {
    width: 3rem;
    margin-right: 0.5rem;
  }
}
</style>
