<template>
    <div>
        <div class="container">
            <ul class="d-flex">
                <li class="d-flex align-items-center py-4" v-for="(content, index) in MainMiddleContent" :key="index">
                    <img :src="content.img" class="py-4" :alt="content.img">
                    <span class="ms-3 me-5">{{content.text}}</span>
                </li>
            </ul>
        </div>
    </div>
</template>

<script>
export default {
    name: 'MainMiddle',
    data() {
        return {
            MainMiddleContent: [
                {
                    img: 'images/buy-comics-digital-comics.png',
                    text: 'DIGITAL COMICS'
                },
                {
                    img: 'images/buy-comics-merchandise.png',
                    text: 'DC MERCHANDISE'
                },
                {
                    img: 'images/buy-comics-subscriptions.png',
                    text: 'SUBSCRIPTION'
                },
                {
                    img: 'images/buy-comics-shop-locator.png',
                    text: 'COMIC SHOP LOCATOR'
                },
                {
                    img: 'images/buy-dc-power-visa.svg',
                    text: 'DIGITAL COMICS'
                },
                
            ]
        }
    }
}
</script>

<style lang="scss" scoped>
@use '../../assets/styles/partials/variables.scss' as *;

*{
    background-color: $link-navbar;
    color: white;
    font-weight: 600;
}
img{
    width: 50px;
}
</style>