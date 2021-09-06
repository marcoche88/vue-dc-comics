<template>
  <div id="app">
    <Header />
    <main>
      <Contents />
    </main>
  </div>
</template>

<script>
import Header from "@/components/Header.vue";
import Contents from "@/components/Contents.vue";

export default {
  name: "App",
  components: {
    Header,
    Contents,
  },
};
</script>

<style lang="scss">
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

.container {
  max-width: 1200px;
  margin: 0 auto;
}

.h-100 {
  height: 100%;
}

body {
  font-family: sans-serif;
}

img {
  max-width: 100%;
  height: auto;
}

li {
  list-style-type: none;
}

li a {
  text-decoration: none;
  color: #666;
}
</style>
