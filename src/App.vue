<template>
  <div id="app">
    <Header />
    <main>
      <Contents />
    </main>
    <footer>
      <FooterTop />
      <FooterBottom />
    </footer>
  </div>
</template>

<script>
import Header from "@/components/Header.vue";
import Contents from "@/components/Contents.vue";
import FooterTop from "@/components/FooterTop.vue";
import FooterBottom from "@/components/FooterBottom.vue";

export default {
  name: "App",
  components: {
    Header,
    Contents,
    FooterTop,
    FooterBottom,
  },
};
</script>

<style lang="scss">
@import "@/assets/scss/style.scss";
</style>
