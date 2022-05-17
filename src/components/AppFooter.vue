<template>
  <footer class="footer">
    <div class="footer__top container">
      <div class="footer__col">
        <h3>DC COMICS</h3>
        <ul class="link-list">
          <li><a href="">ciao</a></li>
          <li><a href="">ciao</a></li>
          <li><a href="">ciao</a></li>
          <li><a href="">ciao</a></li>
          <li><a href="">ciao</a></li>
          <li><a href="">ciao</a></li>
          <li><a href="">ciao</a></li>
        </ul>
        <h3>SHOP</h3>
        <ul class="link-list">
          <li><a href="">ciao</a></li>
          <li><a href="">ciao</a></li>
        </ul>
      </div>
      <div class="footer__col">
        <h3>DC</h3>
        <ul class="link-list">
          <li><a href="">ciao</a></li>
          <li><a href="">ciao</a></li>
          <li><a href="">ciao</a></li>
          <li><a href="">ciao</a></li>
          <li><a href="">ciao</a></li>
          <li><a href="">ciao</a></li>
          <li><a href="">ciao</a></li>
          <li><a href="">ciao</a></li>
          <li><a href="">ciao</a></li>
          <li><a href="">ciao</a></li>
        </ul>
      </div>
      <div class="footer__col">
        <h3>SITES</h3>
        <ul class="link-list">
          <li><a href="">ciao</a></li>
          <li><a href="">ciao</a></li>
          <li><a href="">ciao</a></li>
          <li><a href="">ciao</a></li>
          <li><a href="">ciao</a></li>
        </ul>
      </div>
      <div class="footer__large-col"></div>
    </div>
    <div class="footer__top container"></div>
  </footer>
</template>

<script>
export default {
  name: "AppFooter",
  data() {
    return {
      footerLinks: [
        {
          url: "",
          text: "characters",
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

.footer {
  background-image: url(../assets/img/footer-bg.jpg);
  .container {
    display: flex;
  }
  &__col {
    width: 12%;
    height: 400px;
    padding-top: 2rem;
  }
  &__col {
    h3 {
      color: white;
      margin-bottom: 1rem;
    }
    .link-list {
      margin: 1rem 0;
    }
    li {
      margin: 0.5rem 0;
      a {
        color: $links-color;
      }
    }
  }
  &__large-col {
    width: 64%;
    height: 400px;
    background-image: url(../assets/img/dc-logo-bg.png);
    background-repeat: no-repeat;
    background-position: center;
  }
}
</style>
