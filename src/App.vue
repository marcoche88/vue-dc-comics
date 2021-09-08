<template>
  <div id="app">
    <Header />
    <main>
      <Hero />
      <Contents />
      <ContentsBlue />
    </main>
    <footer>
      <FooterTop />
      <FooterBottom />
    </footer>
  </div>
</template>

<script>
import Header from "./components/Header.vue";
import Contents from "./components/Contents.vue";
import FooterTop from "./components/FooterTop.vue";
import FooterBottom from "./components/FooterBottom.vue";
import ContentsBlue from "./components/ContentsBlue.vue";
import Hero from "./components/Hero.vue";

export default {
  name: "App",
  components: {
    Header,
    Contents,
    FooterTop,
    FooterBottom,
    ContentsBlue,
    Hero,
  },
};
</script>

<style lang="scss">
@import "./assets/scss/style.scss";
</style>
