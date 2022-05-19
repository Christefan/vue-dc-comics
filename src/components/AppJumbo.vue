<template>
  <main>
    <div class="container-jumbo">
      <div class="current-border"></div>
    </div>
    <div class="list-comics">
      <div class="container-comics">
        <ComicsList
          v-for="(items, index) in Arrcomic"
          :key="index"
          :comicsObj="items"
        />
      </div>
    </div>
    <div class="container-shop">
      <ul>
        <li v-for="(items, index) in ArrImg" :key="index">
          <div class="cont">
            <img :src="require(`@/assets/img/${items.url}`)" alt="" />
            <p>{{ items.text }}</p>
          </div>
        </li>
        <!-- <li>
          <div class="cont">
            <img src="../assets/img/buy-comics-digital-comics.png" alt="" />
            <p>Digital Comics</p>
          </div>
        </li>
        <li>
          <div class="cont">
            <img src="../assets/img/buy-comics-merchandise.png" alt="" />
            <p>DC MERCHANDISE</p>
          </div>
        </li>
        <li>
          <div class="cont">
            <img src="../assets/img/buy-comics-shop-locator.png" alt="" />
            <p>SUBSCRIPTION</p>
          </div>
        </li>
        <li>
          <div class="cont">
            <img src="../assets/img/buy-comics-subscriptions.png" alt="" />
            <p>COMIC SHOP LOCATOR</p>
          </div>
        </li>
        <li>
          <div class="cont">
            <img src="../assets/img/buy-dc-power-visa.svg" alt="" />
            <p>DC POWER</p>
          </div>
        </li> -->
      </ul>
    </div>
  </main>
</template>

<script>
import ComicsList from "./ComicsList.vue";

export default {
  name: "AppJumbo",
  components: {
    ComicsList,
  },
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
      Arrcomic: [
        {
          thumb:
            "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/AC1000_DLX_162-001_HD_5ba13723281ab0.37845353.jpg?itok=ZsI-C5eX",
          price: "$19.99",
          series: "Action Comics",
          type: "comic book",
        },
        {
          thumb:
            "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/AV1976_01_300-001_HD_5f738f6e39ddd7.18205602.jpg?itok=VgdYdJ01",
          price: "$3.99",
          series: "American Vampire 1976",
          type: "comic book",
        },
        {
          thumb:
            "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/gn-covers/2018/08/AQMv4_UW_153-001_HD_5b7efa1745a9b8.08589135.jpg?itok=HPTtnrsb",
          price: "$16.99",
          series: "Aquaman",
          type: "graphic novel",
        },
        {
          thumb:
            "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/06/batgirl_v5_1_5b23e1f1124941.50950783.jpg?itok=VnrJah76",
          price: "$2.99",
          series: "Batgirl",
          type: "comic book",
        },
        {
          thumb:
            "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/BM_56_300-001_HD_5ba137a85c3bf3.33122291.jpg?itok=3FHJQYJZ",
          price: "$3.99",
          series: "Batman",
          type: "comic book",
        },
        {
          thumb:
            "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/BM_56_300-001_HD_5ba137a85c3bf3.33122291.jpg?itok=3FHJQYJZ",
          price: "$2.99",
          series: "Batman Beyond",
          type: "comic book",
        },
        {
          thumb:
            "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2019/08/BMSM_5d4361b7116261.74371456.jpg?itok=kEDR2OL8",
          price: "$3.99",
          series: "Batman/Superman",
          type: "comic book",
        },
        {
          thumb:
            "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/BMSMANN_01_300-001_HD_5f5ff17fa1d665.74704970.jpg?itok=azz5sfGk",
          price: "$4.99",
          series: "Batman/Superman Annual",
          type: "comic book",
        },
        {
          thumb:
            "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/BMTJWZ_01_300-001_HD_5f5ff2307dcb37.34652945.jpg?itok=VswVjLR8",
          price: "$5.99",
          series: "Batman: The Joker War Zone",
          type: "comic book",
        },
        {
          thumb:
            "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/08/cover-v2_5f40314645a734.37285065.png?itok=ImNM2QBY",
          price: "$6.99",
          series: "Batman: Three Jokers",
          type: "comic book",
        },
        {
          thumb:
            "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/10/BMWK_HQ_01_300-001_HD_5f7cb4945e13f6.89501032.jpg?itok=sVwALbUX",
          price: "$4.99",
          series: "Batman: White Knight Presents: Harley Quinn",
          type: "comic book",
        },
        {
          thumb:
            "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/gn-covers/2019/04/CTWv1_CC_144-001_HD_5ca5299a751963.53054221.jpg?itok=ooPaoLDq",
          price: "$16.99",
          series: "Catwoman",
          type: "graphic novel",
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
  background-image: url(../assets/img/jumbotron.jpg);
  background-size: cover;
  height: 41vh;
  display: flex;
  align-items: center;
}
.list-comics {
  background-color: rgb(33, 31, 31);
  display: flex;
  .container-comics {
    width: 70%;
    margin: 40px auto 190px;
    display: flex;
    justify-content: space-between;
    flex-wrap: wrap;
    // border: 2px solid blue;

    h5 {
      color: white;
      padding: 0.1em;
      width: 77.8%;
    }
  }
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
