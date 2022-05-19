<template>
  <div class="prova">
    <img :src="comicsObj.thumb" alt="" />
    <h5>{{ comicsObj.series }}</h5>
  </div>
</template>
<script>
export default {
  name: "ComicsList",
  props: {
    comicsObj: Object,
  },
};
</script>
