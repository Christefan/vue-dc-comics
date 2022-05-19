<template>
  <footer>
    <div class="footer-container">
      <div class="footer-nav">
        <ul>
          <li><h2>DC COMICS</h2></li>
          <li><a href="#"> Caracters </a></li>
          <li><a href="#"> Comics </a></li>
          <li><a href="#"> Movies </a></li>
          <li><a href="#"> Tv </a></li>
          <li><a href="#"> Games </a></li>
          <li><a href="#"> Videos </a></li>
          <li><a href="#"> News </a></li>

          <li><h2>SHOP</h2></li>
          <li><a href="#"> Shop DC </a></li>
          <li><a href="#"> Shop DC Collectibles </a></li>
        </ul>
        <ul>
          <li><h2>DC</h2></li>
          <li><a href="#"> Terms of Use </a></li>
          <li><a href="#"> Privacy Policy </a></li>
          <li><a href="#"> Ad Choices </a></li>
          <li><a href="#"> Advertising </a></li>
          <li><a href="#"> Jobs </a></li>
          <li><a href="#"> Subscriptions </a></li>
          <li><a href="#"> Talent Workshops </a></li>
          <li><a href="#"> CPSC Certificates </a></li>
          <li><a href="#"> Ratings </a></li>
          <li><a href="#"> Shop Help </a></li>
          <li><a href="#"> Contact Us </a></li>
        </ul>
        <ul>
          <li><h2>SITES</h2></li>
          <li><a href="#"> DC </a></li>
          <li><a href="#"> MAD Magazine </a></li>
          <li><a href="#"> DC Kid </a></li>
          <li><a href="#"> DC Universe </a></li>
          <li><a href="#"> DC Power Visa </a></li>
        </ul>
      </div>
    </div>
  </footer>
</template>

<script>
export default {
  name: "AppFooter",
};
</script>

<style scoped lang="scss">
footer {
  background-image: url(../assets/img/footer-bg.jpg);
  background-size: cover;
  .footer-container {
    height: 450px;
    width: 90%;
    background-image: url(../assets/img/dc-logo-bg.png);
    background-repeat: no-repeat;
    background-position: right center;
    .footer-nav {
      display: flex;
      h2 {
        color: white;
        font-size: 20px;
      }

      ul {
        list-style-type: none;
        li {
          padding: 5px 0;
          a {
            text-decoration: none;
            color: rgb(155, 152, 152);
            font-size: 14px;
          }
        }
      }
    }
  }
}
</style>
