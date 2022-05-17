<template>
  <section class="social-bg">
    <div class="footer-social">
      <div>
        <button>SIGN-UP NOW</button>
      </div>
      <div class="social-icons">
        <div>FOLLOW US</div>
        <img src="../assets/img/footer-facebook.png" alt="" />
        <img src="../assets/img/footer-twitter.png" alt="" />
        <img src="../assets/img/footer-youtube.png" alt="" />
        <img src="../assets/img/footer-pinterest.png" alt="" />
        <img src="../assets/img/footer-periscope.png" alt="" />
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "AppSocial",
};
</script>

<style lang="scss" scoped>
.social-bg {
  background-color: #333;
  position: relative;
  .footer-social {
    height: 100px;
    width: 80%;
    margin: 0 auto;
    display: flex;
    justify-content: space-between;
    align-items: center;
    button {
      padding: 10px;
      border: 2px #0282f9 solid;
      background-color: #333;
      color: white;
    }
    .social-icons {
      display: flex;
      align-items: center;
      div {
        margin-right: 20px;
        color: blue;
        font-weight: 700;
      }
      img {
        margin: 0 10px;
      }
    }
  }
}
</style>
