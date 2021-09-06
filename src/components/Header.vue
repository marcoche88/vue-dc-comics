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

<style scoped>
header {
  height: 100px;
  display: flex;
  justify-content: space-between;
  align-items: center;
}

figure {
  padding: 20px 0;
  width: 60px;
}

ul {
  display: flex;
  align-items: center;
  justify-content: center;
}

ul li {
  display: inline-block;
  height: 100%;
}

header a {
  display: inline-block;
  padding: 0 10px;
  line-height: 97px;
  font-size: 10px;
  font-weight: bold;
  text-transform: uppercase;
  border-bottom: 3px solid transparent;
}

header a:hover,
header a.active {
  color: rgb(48, 132, 241);
  border-bottom: 3px solid rgb(48, 132, 241);
}
</style>