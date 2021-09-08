<template>
  <section id="contents-blue">
    <div class="container h-100">
      <ul class="row h-100">
        <li v-for="(link, index) in blueLinks" :key="index" class="col">
          <a href="#">
            <img :src="getImageUrl(link.url)" :alt="link.text" />
            <span>{{ link.text }}</span>
          </a>
        </li>
      </ul>
    </div>
  </section>
</template>

<script>
export default {
  name: "ContentsBlue",
  data() {
    return {
      blueLinks: [
        {
          text: "Digital comics",
          url: "buy-comics-digital-comics.png",
        },
        {
          text: "Dc merchandise",
          url: "buy-comics-merchandise.png",
        },
        {
          text: "Subscription",
          url: "buy-comics-subscriptions.png",
        },
        {
          text: "Comic shop locator",
          url: "buy-comics-shop-locator.png",
        },
        {
          text: "Dc power visa",
          url: "buy-dc-power-visa.svg",
        },
      ],
    };
  },
  methods: {
    getImageUrl(url) {
      return require("@/assets/img/" + url);
    },
  },
};
</script>

<style scoped lang="scss">
@import "@/assets/scss/_vars.scss";
@import "@/assets/scss/_mixin.scss";

#contents-blue {
  background-color: $primary-color;
  height: 120px;
}

ul.row {
  @include flex-between;
  margin: 0 20px;
  li.col {
    display: inline-block;
    color: white;
    a {
      @include flex-center;
      color: white;
      img {
        height: 40px;
        margin-right: 10px;
      }
      span {
        text-transform: uppercase;
        font-size: 12px;
      }
    }
  }
}
</style>