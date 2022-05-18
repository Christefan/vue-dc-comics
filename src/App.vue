<template>
  <div id="app">
    <AppHeader />
    <AppJumbo />
    <AppFooter />
    <AppSocial />
  </div>
</template>

<script>
import AppHeader from "./components/AppHeader.vue";
import AppJumbo from "./components/AppJumbo.vue";
import AppFooter from "./components/AppFooter.vue";
import AppSocial from "./components/AppSocial.vue";
export default {
  name: "App",
  components: {
    AppHeader,
    AppJumbo,
    AppFooter,
    AppSocial,
  },
};
</script>

<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
}
</style>
