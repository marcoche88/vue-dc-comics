<template>
  <div id="footer-bottom">
    <div class="container h-100">
      <div class="row h-100">
        <div class="col">
          <div class="button"><a href="#">Sign-up now!</a></div>
        </div>
        <div class="col social">
          <h4>Follow Us</h4>
          <a href="#">
            <img src="@/assets/img/footer-facebook.png" alt="facebook" />
          </a>
          <a href="#">
            <img src="@/assets/img/footer-twitter.png" alt="twitter" />
          </a>
          <a href="#">
            <img src="@/assets/img/footer-youtube.png" alt="youtube" />
          </a>
          <a href="#">
            <img src="@/assets/img/footer-pinterest.png" alt="pinterest" />
          </a>
          <a href="#">
            <img src="@/assets/img/footer-periscope.png" alt="periscope" />
          </a>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "FooterBottom",
};
</script>

<style scoped lang="scss">
@import "@/assets/scss/_vars.scss";

#footer-bottom {
  background-color: rgb(48, 48, 48);
  height: 15vh;
}

.row {
  display: flex;
  justify-content: space-between;
  align-items: center;
}

.button a {
  text-decoration: none;
  color: white;
  text-transform: uppercase;
  font-size: 12px;
  font-weight: bold;
  padding: 12px;
  border: 2px solid $primary-color;
}

.social {
  display: flex;
  flex-basis: 350px;
  justify-content: space-between;
  align-items: center;
  a {
    display: inline-block;
  }
}

h4 {
  text-transform: uppercase;
  color: $primary-color;
}
</style>