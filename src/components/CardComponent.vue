<template>
  
  <div class="">
    <div class="card">
    <img :src="thumb" class="card-img-top" :alt="series">
    
  </div>
  <div class="card-body">
      <h5 class="card-series">{{ series }}</h5>
    </div>
  </div>
</template>

<script>

export default {
  name: 'CardComponent',
  props: {
    thumb: String,
    series: String,
  },
};
</script>

<style lang="scss" scoped>
  .card{
    img{
      height: 300px;
    }
  }

</style>
