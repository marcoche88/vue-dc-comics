<template>
  <header class="container">
    <figure>
      <img src="@/assets/img/dc-logo.png" alt="logo" />
    </figure>
    <nav class="h-100">
      <ul>
        <li v-for="(link, index) in links" :key="index">
          <a :href="link.url" :class="{ active: link.current }">{{
            link.text
          }}</a>
        </li>
      </ul>
    </nav>
  </header>
</template>

<script>
export default {
  name: "Header",
  data() {
    return {
      links: [
        {
          text: "Characters",
          url: "#",
          current: false,
        },
        {
          text: "Comics",
          url: "#",
          current: true,
        },
        {
          text: "Movies",
          url: "#",
          current: false,
        },
        {
          text: "TV",
          url: "#",
          current: false,
        },
        {
          text: "Games",
          url: "#",
          current: false,
        },
        {
          text: "Collectibles",
          url: "#",
          current: false,
        },
        {
          text: "Videos",
          url: "#",
          current: false,
        },
        {
          text: "Fans",
          url: "#",
          current: false,
        },
        {
          text: "News",
          url: "#",
          current: false,
        },
        {
          text: "Shop",
          url: "#",
          current: false,
        },
      ],
    };
  },
};
</script>

<style lang="scss" scoped>
@import "@/assets/scss/_vars.scss";
@import "@/assets/scss/_mixin.scss";

header {
  height: 15vh;
  @include flex-between;
  a {
    display: inline-block;
    padding: 0 10px;
    line-height: calc(15vh - 3px);
    font-size: 12px;
    font-weight: bold;
    text-transform: uppercase;
    border-bottom: 3px solid transparent;
    &:hover,
    &.active {
      color: $primary-color;
      border-bottom: 3px solid $primary-color;
    }
  }
}

figure {
  width: 80px;
}

ul {
  @include flex-center;
  li {
    display: inline-block;
    height: 100%;
  }
}
</style>