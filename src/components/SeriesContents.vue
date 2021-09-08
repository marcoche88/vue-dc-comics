<template>
  <section class="series-contents container">
    <div class="title">current series</div>
    <div class="series">
      <CardSeries
        v-for="(comic, index) in dcComics"
        :key="index"
        :comic="comic"
      />
    </div>
    <div class="load-more">
      <div class="button-load pointer">load more</div>
    </div>
  </section>
</template>

<script>
import CardSeries from "./CardSeries.vue";
import dcComics from "../data/dcComics.js";

export default {
  name: "SeriesContents",
  data() {
    return {
      dcComics,
    };
  },
  components: {
    CardSeries,
  },
};
</script>

<style scoped lang="scss">
@import "../assets/scss/_vars.scss";
.series-contents {
  position: relative;
}

.title {
  background-color: $primary-color;
  padding: 10px 30px;
  font-size: 22px;
  text-transform: uppercase;
  font-weight: bold;
  position: absolute;
  left: 0;
  top: -20px;
}

.series {
  padding-top: 50px;
  display: flex;
  justify-content: center;
  flex-wrap: wrap;
}

.load-more {
  text-align: center;
  padding: 25px;
  .button-load {
    display: inline-block;
    padding: 10px 50px;
    text-transform: uppercase;
    font-weight: bold;
    font-size: 12px;
    background-color: $primary-color;
  }
}
</style>