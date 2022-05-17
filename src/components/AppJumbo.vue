<template>
  <main>
    <div class="container-jumbo">
      <p>--> Content goes here --</p>
    </div>
    <div class="container-shop">
      <ul>
        <!-- <li>
          <div class="cont" v-for="(items, index) in ArrImg" :key="index">
            <img src="../assets/img/'items.url'" alt="" />
            <p>{{ items.text }}</p>
          </div>
        </li> -->
        <li>
          <div class="cont">
            <img src="../assets/img/buy-comics-digital-comics.png" alt="" />
            <p>Digital Comics</p>
          </div>
        </li>
        <li>
          <div class="cont">
            <img src="../assets/img/buy-comics-merchandise.png" alt="" />
            <p>Digital Comics</p>
          </div>
        </li>
        <li>
          <div class="cont">
            <img src="../assets/img/buy-comics-shop-locator.png" alt="" />
            <p>Digital Comics</p>
          </div>
        </li>
        <li>
          <div class="cont">
            <img src="../assets/img/buy-comics-subscriptions.png" alt="" />
            <p>Digital Comics</p>
          </div>
        </li>
        <li>
          <div class="cont">
            <img src="../assets/img/buy-dc-power-visa.svg" alt="" />
            <p>Digital Comics</p>
          </div>
        </li>
      </ul>
    </div>
  </main>
</template>

<script>
export default {
  name: "AppJumbo",
  data() {
    return {
      ArrImg: [
        {
          url: "buy-comics-digital-comics.png",
          text: "DIGITAL COMICS",
        },
        {
          url: "buy-comics-merchandise.png",
          text: "DC MERCHANDISE",
        },
        {
          url: "buy-comics-shop-locator.png",
          text: "SUBSCRIPTION",
        },
        {
          url: "buy-comics-subscriptions.png",
          text: "COMIC SHOP LOCATOR",
        },
        {
          url: "buy-dc-power-visa.svg",
          text: "DC POWER",
        },
      ],
    };
  },
};
</script>

<style lang="scss" scoped>
main {
  position: relative;
}
.container-jumbo {
  background-color: black;
  height: 100px;
  display: flex;
  align-items: center;
}
p {
  color: white;
  margin-left: 50px;
}
.container-shop {
  background-color: blue;
  height: 20vh;
  display: flex;
  align-items: center;
  justify-content: space-around;
  ul {
    display: flex;
  }
  li {
    list-style-type: none;
    margin: 0 15px;
  }
  img {
    width: 60px;
    height: 60px;
  }
  .cont {
    display: flex;
    align-items: center;

    p {
      font-size: 20px;
      margin: 0 10px;
    }
  }
}
</style>
