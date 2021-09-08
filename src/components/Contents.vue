<template>
  <section id="contents">
    <SeriesContents />
  </section>
</template>

<script>
import SeriesContents from "./SeriesContents.vue";

export default {
  name: "Contents",
  components: {
    SeriesContents,
  },
};
</script>

<style scoped lang="scss">
#contents {
  background-color: rgb(28, 28, 28);
  color: white;
}
</style>