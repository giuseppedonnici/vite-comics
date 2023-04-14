<script>
import AppContent from './AppContent.vue';
export default {
    name: "AppMain",
    components: {
        AppContent
    },
    data() {
        return {
            ctaArray: [
                {
                    image: "buy-comics-digital-comics.png",
                    title: "digital comics"
                },
                {
                    image: "buy-comics-merchandise.png",
                    title: "dc merchandise"
                },
                {
                    image: "buy-comics-subscriptions.png",
                    title: "subscription"
                },
                {
                    image: "buy-comics-shop-locator.png",
                    title: "comic shop locator"
                },
                {
                    image: "buy-dc-power-visa.svg",
                    title: "dc power visa"
                }
            ]
        }
    },
    methods: {
        getImagePath(imageName) {
            return new URL(`../assets/img/${imageName}`, import.meta.url).href;
        }
    }
}
</script>

<template>
    <main>
        <div class="jumbotron">

        </div>

        <div class="content">
            <div class="container">
            <a class=" btn" href="#">CURRENT SERIES</a>
            <AppContent />
            </div>
        </div>

        <div class="cta">
            <div class="container">
                <ul>
                    <li v-for="cta in ctaArray">
                        <a href="#">
                            <img :src="getImagePath( cta.image )" alt="">
                            <span>{{ cta.title }}</span>
                        </a>
                    </li>
                </ul>
            </div>
        </div>
    </main>
</template>

<style scoped lang="scss">
@use "../style/partials/variables" as *;


main {
    .jumbotron {
        height: 300px;
        background-image: url(../assets/img/jumbotron.jpg);
        background-size: cover;
    }

    .container {
        position: relative;
    }
    a {
        &.btn {
            display: inline-block;
            position: absolute;
            top: -50px;
            left: 0;
            padding: 10px 25px;
            background-color: $primary;
        }
    }
    .content {
        color: white;
        padding: 2rem 0;
        font-weight: bold;
        font-stretch: ultra-condensed;
        background-color: black;
    }
    
    .cta {
        position: relative;
        z-index: 1;
        height: 150px;
        color: white;
        background-color: $primary;
        ul {
            display: flex;
            align-items: center;
            justify-content: center;
            gap: 3rem;
            height: 100%;
        }
        img {
            width: 45px;
            vertical-align: middle;
        }
        span {
            display: inline-block;
            font-size: .7rem;
            text-transform: uppercase;
            padding-left: .7rem;
        }
    }
}
</style>