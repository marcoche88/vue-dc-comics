<template>
  <div class="card">
    <img :src="comic.thumb" :alt="comic.series" />
    <figcaption>{{ comic.series }}</figcaption>
  </div>
</template>

<script>
export default {
  name: "CardSeries",
  props: ["comic"],
};
</script>

<style scoped lang="scss">
.card {
  flex-basis: calc(100% / 6);
  padding-bottom: 40px;
  padding-left: 10px;
  padding-right: 10px;
  img {
    width: 100%;
    height: 180px;
    object-fit: cover;
    object-position: top;
  }
  figcaption {
    margin-top: 20px;
    text-transform: uppercase;
    font-size: 13px;
    color: rgba(255, 255, 255, 0.8);
  }
}
</style>