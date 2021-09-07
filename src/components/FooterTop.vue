<template>
  <div id="footer-top">
    <div class="container h-100">
      <div class="row h-100">
        <div class="col footer-left">
          <div class="col">
            <h5>Dc Comics</h5>
            <ul>
              <li><a href="#">Characters</a></li>
              <li><a class="active" href="#">Comics</a></li>
              <li><a href="#">Movies</a></li>
              <li><a href="#">Tv</a></li>
              <li><a href="#">Games</a></li>
              <li><a href="#">Videos</a></li>
              <li><a href="#">News</a></li>
            </ul>
            <h5 class="shop">Shop</h5>
            <ul>
              <li><a href="#">Shop DC</a></li>
              <li><a class="active" href="#">Shop DC Collectibles</a></li>
            </ul>
          </div>
          <div class="col">
            <h5>Dc</h5>
            <ul>
              <li><a href="#">Term Of Use</a></li>
              <li><a class="active" href="#">Privacy Policy (New)</a></li>
              <li><a href="#">Ad Choices</a></li>
              <li><a href="#">Advertising</a></li>
              <li><a href="#">Jobs</a></li>
              <li><a href="#">Subscriptions</a></li>
              <li><a href="#">Talent Workshops</a></li>
              <li><a href="#">CPSC Certificates</a></li>
              <li><a href="#">Ratings</a></li>
              <li><a href="#">Shop Help</a></li>
              <li><a href="#">Contact Us</a></li>
            </ul>
          </div>
          <div class="col">
            <h5>Sites</h5>
            <ul>
              <li><a href="#">DC</a></li>
              <li><a class="active" href="#">MAD Magazine</a></li>
              <li><a href="#">DC Kids</a></li>
              <li><a href="#">Dc Universe</a></li>
              <li><a href="#">DC Power Visa</a></li>
            </ul>
          </div>
        </div>
        <div class="col footer-right">
          <img src="@/assets/img/dc-logo-bg.png" alt="logo-bg" />
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "FooterTop",
};
</script>

<style scoped lang="scss">
#footer-top {
  height: 40vh;
  background-image: url("../assets/img/footer-bg.jpg");
  background-position: top;
  background-repeat: no-repeat;
  background-size: cover;
  overflow: hidden;
  img {
    height: 450px;
  }
}

.row {
  color: white;
  display: flex;
  justify-content: space-between;
}

.footer-left {
  display: flex;
  margin-top: 30px;
  .col {
    margin-right: 40px;
  }
  h5 {
    text-transform: uppercase;
    margin-bottom: 10px;
  }
  h5.shop {
    margin-top: 15px;
  }
  a {
    font-size: 10px;
  }
}

.footer-right {
  align-self: center;
}
</style>