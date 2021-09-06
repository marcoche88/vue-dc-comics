<template>
  <header class="container">
    <figure>
      <img src="@/assets/img/dc-logo.png" alt="logo" />
    </figure>
    <nav class="h-100">
      <ul>
        <li><a href="#">Characters</a></li>
        <li><a class="active" href="#">Comics</a></li>
        <li><a href="#">Movies</a></li>
        <li><a href="#">Tv</a></li>
        <li><a href="#">Games</a></li>
        <li><a href="#">Collectibles</a></li>
        <li><a href="#">Videos</a></li>
        <li><a href="#">Fans</a></li>
        <li><a href="#">News</a></li>
        <li><a href="#">Shop</a></li>
      </ul>
    </nav>
  </header>
</template>

<script>
export default {
  name: "Header",
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