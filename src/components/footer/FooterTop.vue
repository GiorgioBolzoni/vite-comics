<template>
    <div class="bg-footer py-4">
        <div class="container">
                <div class="row">
                    <div class="col-3" v-for="item, index in menu" :key="index">
                        <h4 class="fw-bold">{{ item.title }}</h4>
                        <div>
                            <ul class="justify-content-start">
                                <li v-for="(link, index) in item.links" :key="index"><a :href="link.url">{{ link.text }}</a>
                                </li>
                            </ul>
                        </div>

                    </div>
                    <div class="col-3">
                        <img src="/images/dc-logo-bg.png" alt="dc-logo-bg.png" id="logo-bg">
                    </div>
                </div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'FooterTop',
    data() {
        return {
            menu: [
                {
                    title: 'DC COMICS',
                    links: [
                        {
                            text: "Characters",
                            url: "#",
                        },
                        {
                            text: "Comics",
                            url: "#",
                        },
                        {
                            text: "Movies",
                            url: "#",
                        },
                        {
                            text: "TV",
                            url: "#",
                        },
                        {
                            text: "Games",
                            url: "#",
                        },
                        {
                            text: "Videos",
                            url: "#",
                        },
                        {
                            text: "News",
                            url: "#",
                        }
                    ],
                    title: 'SHOP',
                    links: [
                        {
                            text: "Shop DC",
                            url: "#",
                        },
                        {
                            text: "Shop DC Collectibles",
                            url: "#",
                        }
                    ]
                },
                {
                    title: 'DC',
                    links: [
                        {
                            text: "Term Of Use",
                            url: "#",
                        },
                        {
                            text: "Privacy policy (New)",
                            url: "#",
                        },
                        {
                            text: "Ad Choices",
                            url: "#",
                        },
                        {
                            text: "Advertising",
                            url: "#",
                        },
                        {
                            text: "Jobs",
                            url: "#",
                        },
                        {
                            text: "Subscriptions",
                            url: "#",
                        },
                        {
                            text: "Talent Workshops",
                            url: "#",
                        },
                        {
                            text: "CPSC Certificates",
                            url: "#",
                        },
                        {
                            text: "Ratings",
                            url: "#",
                        },
                        {
                            text: "Shop Help",
                            url: "#",
                        },
                        {
                            text: "Contact Us",
                            url: "#",
                        }
                    ]
                },
                {
                    title: 'SITES',
                    links: [
                        {
                            text: "DC",
                            url: "#",
                        },
                        {
                            text: "MAD Magazine",
                            url: "#",
                        },
                        {
                            text: "DC Kids",
                            url: "#",
                        },
                        {
                            text: "DC Universe",
                            url: "#",
                        },
                        {
                            text: "DC Power Visa",
                            url: "#",
                        }
                    ]
                },

            ]
        }
    }
}
</script>

<style lang="scss" scoped>
@use '../../assets/styles/partials/variables' as *;
.bg-footer{
    background-image: url(../../assets/images/footer-bg.jpg);
    color: white;
    background-repeat: no-repeat;
    background-position: bottom;
    background-size: cover;
    position: relative  ;}
li{
    list-style: none;
    a{
        color: rgb(134, 134, 134);
        text-decoration: none;
        margin-left: -32px;
        &:hover {
                    color: white;
                }
    }
}
</style>