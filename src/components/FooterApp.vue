<template>
    <footer>
        <section class="footer-top">
            <FooterTop />
        </section>
        <section class="footer-bottom">
            <FooterBottom />
        </section>
    </footer>
</template>

<script>
import FooterTop from './footer/FooterTop.vue'
import FooterBottom from './footer/FooterBottom.vue'

export default {
    name: 'FooterApp',
    components: {
      FooterTop,
      FooterBottom
    }
};
</script>

<style lang="scss" scoped>
@use '../assets/styles/partials/variables' as *;
.footer-top{
    margin-top: -16px;
}


</style>