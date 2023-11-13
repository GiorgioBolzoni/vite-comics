<template>
    <div class="container">
        <div class="row">
            <div class="col-12 col-md-4 col-lg-2" v-for="(tvSerie, index) in tvSeries" :key="index">
                <CardComponent :img="tvSerie.thumb" :title="tvSerie.series" />
            </div>
        </div>
    </div>
</template>

<script>
import seriesTV from '../../data/dcComics'
import CardComponent from '../CardComponent.vue';

export default {
    name: 'MainTop',
    components:{
        CardComponent
    },
    data(){
        return{
            tvSeries: seriesTV,
        }
    }
}
</script>

<style lang="scss" scoped>
@use '../../assets/styles/partials/variables' as *;

</style>