<template>
  <footer class="footer">
    <div class="footer__top container">
      <div class="footer__col">
        <h3>DC COMICS</h3>
        <AppLinks
          v-for="(item, index) in footerLinksDcComics"
          :key="index"
          :linkObj="item"
        />
        <h3>SHOP</h3>
        <AppLinks
          v-for="(item, index) in footerLinksShop"
          :key="index"
          :linkObj="item"
        />
      </div>
      <div class="footer__col">
        <h3>DC</h3>
        <AppLinks
          v-for="(item, index) in footerLinksDC"
          :key="index"
          :linkObj="item"
        />
      </div>
      <div class="footer__col">
        <h3>SITES</h3>
        <AppLinks
          v-for="(item, index) in footerLinksSites"
          :key="index"
          :linkObj="item"
        />
      </div>
      <div class="footer__large-col"></div>
    </div>
    <div class="footer__bottom">
      <div class="container">
        <div class="footer__sign-up">
          <button>SIGN-UP NOW!</button>
        </div>
        <div class="footer__social-box">
          <div class="follow-us">FOLLOW US</div>
          <ul class="social-box-btn">
            <li v-for="(item, index) in footerSocial" :key="index">
              <a href=""
                ><img :src="require(`../assets/img/${item.src}.png`)" alt="" />
              </a>
            </li>
          </ul>
        </div>
      </div>
    </div>
  </footer>
</template>

<script>
import AppLinks from "../components/AppLinks.vue";
export default {
  name: "AppFooter",
  components: {
    AppLinks,
  },
  data() {
    return {
      footerLinksDcComics: [
        {
          url: "",
          text: "Characters",
        },
        {
          url: "",
          text: "Comics",
        },
        {
          url: "",
          text: "Movies",
        },
        {
          url: "",
          text: "TV",
        },
        {
          url: "",
          text: "Games",
        },
        {
          url: "",
          text: "Videos",
        },
        {
          url: "",
          text: "News",
        },
      ],
      footerLinksShop: [
        {
          url: "",
          text: "Shop DC",
        },
        {
          url: "",
          text: "Shop DC Collectibles",
        },
      ],
      footerLinksDC: [
        {
          url: "",
          text: "Terms Of Use",
        },
        {
          url: "",
          text: "Privacy policy (New)",
        },
        {
          url: "",
          text: "Ad Choices",
        },
        {
          url: "",
          text: "Advertsing",
        },
        {
          url: "",
          text: "Jobs",
        },
        {
          url: "",
          text: "Subscriptions",
        },
        {
          url: "",
          text: "Talent Workshops",
        },
        {
          url: "",
          text: "CPSC Certificates",
        },
        {
          url: "",
          text: "Ratings",
        },
        {
          url: "",
          text: "Shop Help",
        },
        {
          url: "",
          text: "Contact Us",
        },
      ],
      footerLinksSites: [
        {
          url: "",
          text: "DC",
        },
        {
          url: "",
          text: "MAD Magazine",
        },
        {
          url: "",
          text: "DC Kids",
        },
        {
          url: "",
          text: "DC Universe",
        },
        {
          url: "",
          text: "DC Power Visa",
        },
      ],
      footerSocial: [
        {
          name: "facebook",
          src: "footer-facebook",
        },
        {
          name: "twitter",
          src: "footer-twitter",
        },
        {
          name: "youtube",
          src: "footer-youtube",
        },
        {
          name: "pintarest",
          src: "footer-pinterest",
        },
        {
          name: "periscope",
          src: "footer-periscope",
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
      margin: 1rem 0;
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
  &__bottom {
    background-color: #303030;
    height: 100px;
    color: white;
    display: flex;
    .container {
      justify-content: space-between;
      align-items: center;
    }
  }
  &__sign-up button {
    color: white;
    background-color: transparent;
    padding: 1rem;
    border: 2px solid $brand-primary-color;
  }
  &__social-box {
    display: flex;
    align-items: center;
    .follow-us {
      color: $brand-primary-color;
      font-size: 1.1rem;
      font-weight: 700;
      margin: 0 1rem;
    }
    ul {
      display: flex;
      li {
        margin: 0 0.5rem;
      }
    }
  }
}
</style>
