<template>
  <div class="comic">
    <img :src="comic.thumb" :alt="comic.series" />
    <h5>{{ comic.series }}</h5>
  </div>
</template>

<script>
export default {
  name: "ComicProduct",
  props: {
    comic: Object,
  },
};
</script>

<style scoped lang="scss">
.comic {
  width: 200px;
  height: fit-content;
  text-align: left;

  img {
    margin-bottom: 15px;
    width: 100%;
    height: 200px;
    object-fit: cover;
    object-position: 0 0;
  }

  h5 {
    font-size: 0.9rem;
    font-family: "Roboto", sans-serif;
    font-weight: normal;
    text-transform: uppercase;
  }
}
</style>
