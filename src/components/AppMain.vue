<script>
import AppContent from './AppContent.vue';
export default {
    name: "AppMain",
    components: {
        AppContent
    }
}
</script>

<template>
    <main>
        <div class="jumbotron">

        </div>

        

        <div class="content">
            <div class="container">
            --> Content goes here &lt;--
            <AppContent />
            </div>
        </div>

        <div class="cta">
            <div class="container">
                <ul>
                    <li>
                        <a href="#">
                            <img src="../assets/img/buy-comics-digital-comics.png" alt="">
                            <span>DIGITAL COMICS</span>
                        </a>
                    </li>
                    <li>
                        <a href="#">
                            <img src="../assets/img/buy-comics-merchandise.png" alt="">
                            <span>DC MERCHANDISE</span>
                        </a>
                    </li>
                    <li>
                        <a href="#">
                            <img src="../assets/img/buy-comics-subscriptions.png" alt="">
                            <span>SUBSCRIPTION</span>
                        </a>
                    </li>
                    <li>
                        <a href="#">
                            <img src="../assets/img/buy-comics-shop-locator.png" alt="">
                            <span>COMIC SHOP LOCATOR</span>
                        </a>
                    </li>
                    <li>
                        <a href="#">
                            <img src="../assets/img/buy-dc-power-visa.svg" alt="">
                            <span>DC POWER VISA</span>
                        </a>
                    </li>
                </ul>

            </div>
        </div>
    </main>
</template>

<style scoped lang="scss">
@use "../style/partials/variables" as *;

.jumbotron {
    height: 300px;
    background-image: url(../assets/img/jumbotron.jpg);
    background-size: cover;
}

main {
    .content {
        color: white;
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
            padding-left: .7rem;
        }
    }
}
</style>