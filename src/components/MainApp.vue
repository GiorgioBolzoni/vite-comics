// MainApp.vue

<template>
  <main>
    <section class="jumbotron">
    </section>

    <section class="main-top">
      <div class="container">
        <div class="row">
          <div class="col-2" style="cursor:pointer" v-for="(tvSerie, index) in tvSeries" :key="index">
            <CardComponent :thumb="tvSerie.thumb" :series="tvSerie.series" />
          </div>
        </div>
      </div>
    </section>
    <section class="main-middle">
      <MainMiddle />
    </section>
  </main>
</template>

<script>
import MainMiddle from './main/MainMiddle.vue';
import CardComponent from './CardComponent.vue';
import seriesTV from '../data/dcComics'; 

export default {
  name: 'MainApp',
  components: {
    CardComponent,
    MainMiddle,
  },
  data() {
    return {
      tvSeries: seriesTV,
    };
  },
};
</script>

<style lang="scss" scoped>
@use '../assets/styles/partials/variables' as *;

.main-top {
  background-color: black;
  color: white;
  padding: 50px;

  .col-2 {
    margin-bottom: 20px;
  }
}
.jumbotron {
  background-image: url('../assets/images/jumbotron.jpg');
  height: 400px;
}




</style>
