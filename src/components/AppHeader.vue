<template>
  <div class="header-container">
    <div class="logo">
      <img src="../assets/img/dc-logo.png" alt="" />
    </div>
    <div class="list-header">
      <ul>
        <li v-for="(items, index) in ArrText" :key="index">
          <a href="">{{ items.text }}</a>
        </li>
        <!-- <li>CHARACTERS</li>
        <li>COMICS</li>
        <li>MOVIES</li>
        <li>TV</li>
        <li>GAMES</li>
        <li>COLLECTIBILES</li>
        <li>VIDEOS</li>
        <li>FANS</li>
        <li>NEWS</li>
        <li>SHOP</li> -->
      </ul>
    </div>
  </div>
</template>

<script>
export default {
  name: "AppHeader",
  data() {
    return {
      ArrText: [
        {
          text: "Characters",
        },
        {
          text: "Comics",
        },
        {
          text: "Movies",
        },
        {
          text: "TV",
        },
        {
          text: "Games",
        },
        {
          text: "Collectibles",
        },
        {
          text: "Videos",
        },
        {
          text: "Fans",
        },
        {
          text: "News",
        },
        {
          text: "Shop",
        },
      ],
    };
  },
};
</script>

<style scoped lang="scss">
.header-container {
  display: flex;
  align-items: center;
  justify-content: space-around;
  height: 100px;
  margin-bottom: 20px;
}

.list-header {
  ul {
    display: flex;
  }
  li {
    list-style-type: none;
    margin: 0 15px;
  }
  a {
    text-decoration: none;
    color: black;
  }
  a:hover {
    color: royalblue;
    border-bottom: 5px solid royalblue;
  }
}
</style>
