<template>
  <div class="product">
    <div class="product__img">
      <img :src="productObj.thumb" alt="" />
    </div>
    <small class="product__text">{{ productObj.series }}</small>
  </div>
</template>

<script>
export default {
  name: "AppProduct",
  props: {
    productObj: Object,
  },
};
</script>

<style lang="scss" scoped>
.product {
  width: calc(100% / 6 - 10px);
  color: white;
  padding-bottom: 2rem;
  text-transform: uppercase;
  font-size: 0.8rem;
  &__img {
    max-height: 200px;
    overflow: hidden;
    margin-bottom: 1rem;
    img {
      width: 100%;
    }
  }
  // &__text {
  //   padding: 3rem 0;
  // }
}
</style>
