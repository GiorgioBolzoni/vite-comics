<template>
    
    <main>
        <section class="main-top">
            <MainTop />
        </section>
        <section class="main-middle">
            <MainMiddle />
        </section>
        <section class="main-bottom">
            <MainBottom />
        </section>
    </main>
</template>

<script>
import MainTop from './main/MainTop.vue'
import MainMiddle from './main/MainMiddle.vue'
import MainBottom from './main/MainBottom.vue'

export default {
    name: 'MainApp',
    components: {
      MainTop,
      MainMiddle,
      MainBottom
    }
};
</script>

<style lang="scss" scoped>
@use '../assets/styles/partials/variables' as *;

.main-top {
    background-color: black;
    color: white;
    padding: 50px;
}
</style>