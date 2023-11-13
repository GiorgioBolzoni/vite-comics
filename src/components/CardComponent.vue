<template>
    <div class="card">
  <img :src="thumb" class="card-img-top" :alt="series">
  <div class="card-body">
    <h5 class="card-series">{{series}}</h5>
    
  </div>
</div>
</template>

<script>

export default {
    name: 'CardComponent',
    props:[
        'thumb',
        'series'
    ]
}
</script>

<style lang="scss" scoped>

</style>