<template>
  <section id="contents-blue">
    <div class="container h-100">
      <ul class="row h-100">
        <li class="col">
          <a href="#">
            <img
              src="@/assets/img/buy-comics-digital-comics.png"
              alt="digital comics"
            />
            <span>Digital comics</span>
          </a>
        </li>
        <li class="col">
          <a href="#">
            <img
              src="@/assets/img/buy-comics-merchandise.png"
              alt="merchandise"
            />
            <span>Dc merchandise</span>
          </a>
        </li>
        <li class="col">
          <a href="#">
            <img
              src="@/assets/img/buy-comics-subscriptions.png"
              alt="subscription"
            />
            <span>subscription</span>
          </a>
        </li>
        <li class="col">
          <a href="#">
            <img
              src="@/assets/img/buy-comics-shop-locator.png"
              alt="shop-locator"
            />
            <span>Comic shop locator</span>
          </a>
        </li>
        <li class="col">
          <a href="#">
            <img src="@/assets/img/buy-dc-power-visa.svg" alt="visa" />
            <span>Dc power visa</span>
          </a>
        </li>
      </ul>
    </div>
  </section>
</template>

<script>
export default {
  name: "ContentsBlue",
};
</script>

<style scoped lang="scss">
@import "@/assets/scss/_vars.scss";

#contents-blue {
  background-color: $primary-color;
  height: 120px;
}

ul.row {
  display: flex;
  justify-content: space-between;
  align-items: center;
  margin: 0 20px;
}

ul.row li {
  display: inline-block;
  color: white;
}

ul.row li a {
  display: flex;
  color: white;
  align-items: center;
}

a img {
  height: 40px;
  margin-right: 10px;
}

a span {
  text-transform: uppercase;
  font-size: 12px;
}
</style>