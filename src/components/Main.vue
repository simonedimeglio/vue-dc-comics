<template>
  <div class="main-full">
    <div class="jumbotron">
      <img src="../assets/jumbotron.jpg" alt="Jumbotron">
    </div>
    <div class="container">
      <div class="current">
        <span>CURRENT SERIES</span>
      </div>
      <div class="row">
        <Card
          v-for="(element, index) in comics"
          :key="index"
          :thumb="element.thumb"
          :price="element.price"
          :title="element.series"
          :type="element.type"
        />
      </div>
    </div>
  </div>
</template>

<script>
import Card from './Card.vue';

export default {
  name: "Main",
  components: {
    Card,
  },
  props: {
    comics: Array,
  }
};
</script>

<style lang="scss" scoped>
// @import "../style/colors.scss";
.main-full {
  background: rgba(28, 28, 28, 255);
  color: white;
  .container {
  .current {
    span {
      background-color: rgba(2, 130, 249, 255);
      height: 30px;
      padding: 10px;
    }
  }
}
}

.jumbotron {
  overflow: hidden;
  height: 230px;
  img {
    width: 100%;
  }


  
}
</style>