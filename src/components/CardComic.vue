<template>
  <div class="col-2">
    <div class="comic-container">
      <div
        class="container-img"
        :style="{ backgroundImage: 'url(' + thumb + ')' }"
      ></div>
      <div class="container-text">
        <div>{{ series.toUpperCase() }}</div>
        <div>{{ price }}</div>
        <div>{{ type }}</div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'CardComic',
  props: {
    thumb: String,
    price: Number,
    series: String,
    type: String,
  },
}
</script>

<style lang="scss" scoped>
@import '../style/colors.scss';
@import '../style/fonts.scss';

.col-2 {
  width: calc((100% / 6) - 40px);
  padding: 30px 0;

  .container-img {
    width: 200px;
    height: 150px;
    background-position: top;
    background-size: cover;
  }

  .container-text {
    width: 200px;
    font-size: 12px;
    font-weight: 300;
    margin-top: 10px;
  }
}
</style>
