<template>
  <div class="container">
    <div class="content">
      <div class="row">
        <CardComic
          v-for="(element, index) in comics"
          :key="index"
          :thumb="element.thumb"
          :price="element.price"
          :series="element.series"
          :type="element.type"
        />
      </div>
    </div>
  </div>
</template>

<script>
import CardComic from '@/components/CardComic.vue'

export default {
  name: 'Main',
  components: {
    CardComic,
  },
  props: {
    comics: Array,
  },
  created() {
    console.log(this.comics)
  },
}
</script>

<style lang="scss" scoped>
@import '../style/colors.scss';
@import '../style/fonts.scss';

.content {
  background-color: $bg-color;
  color: $bg-font-color;
  font-weight: 700;
  font-size: 20px;

  .row {
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    align-items: center;
  }

  .main-content {
    width: 65%;
  }
}
</style>
