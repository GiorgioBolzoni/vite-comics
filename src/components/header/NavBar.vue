<template>
    <nav class="d-flex">
        <ul class="nav justify-content-center">
            <li class="nav-item d-flex" v-for="(link, index) in menu" :key="index">
                <a class="nav-link d-flex align-items-center py-5" :href="link.url" :class="{ 'active': link.current}"> {{ link.text }}</a>
            </li>
        </ul>
    </nav>
</template>

<script>
export default {
    name: 'NavBar',
    data() {
        return {
            menu: [
                {
                    text: "characters",
                    url: "#",
                    current: false,
                },
                {
                    text: "comics",
                    url: "#",
                    current: true,
                },
                {
                    text: "movies",
                    url: "#",
                    current: false,
                },
                {
                    text: "tv",
                    url: "#",
                    current: false,
                },
                {
                    text: "games",
                    url: "#",
                    current: false,
                },
                {
                    text: "collectibles",
                    url: "#",
                    current: false,
                },
                {
                    text: "videos",
                    url: "#",
                    current: false,
                },
                {
                    text: "fans",
                    url: "#",
                    current: false,
                },
                {
                    text: "news",
                    url: "#",
                    current: false,
                },
                {
                    text: "shop",
                    url: "#",
                    current: false,
                },
            ]
        }
    }
}
</script>

<style lang="scss" scoped>
@use '../../assets/styles/partials/variables' as *;

    nav{
        height: 200px;
    }
    .nav-link{
    color: black;
    text-transform: uppercase;
    font-weight: 600;
    cursor: pointer;
    border: 10px solid transparent;

        &.active,
        &:hover{
            color: $link-navbar;
            border-bottom: 10px solid $link-navbar;
        };
    }

    
    
 
</style>