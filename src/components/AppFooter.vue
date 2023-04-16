<script>
export default {
    name: "AppFooter",
    data() {
        return {
            
        }
    }
}
</script>

<template>
    <footer>
        <div class="up">
            <div class="container">
                <img src="../assets/img/dc-logo-bg.png" alt="">
                <div class="row">
                    <div class="col left">
                        <ul>
                            <li>
                                <h3>
                                    dc comics
                                </h3>
                            </li>
                            <li>Characters</li>
                            <li>Comics</li>
                            <li>Movies</li>
                            <li>TV</li>
                            <li>Games</li>
                            <li>Videos</li>
                            <li>News</li>
                        </ul>
                        <ul>
                            <li>
                                <h3>
                                    shop
                                </h3>
                            </li>
                            <li>Shop DC</li>
                            <li>Shop DC Collectibles</li>
                        </ul>
                    </div>

                    <div class="col center">
                        <ul>
                            <li>
                                <h3>
                                    dc
                                </h3>
                            </li>
                            <li>Terms Of Use</li>
                            <li>Privacy policy (New)</li>
                            <li>Ad Choices</li>
                            <li>Advertising</li>
                            <li>Jobs</li>
                            <li>Subscriptions</li>
                            <li>Talent Workshops</li>
                            <li>CPSC Certificates</li>
                            <li>Ratings</li>
                            <li>Shop Help</li>
                            <li>Contact Us</li>
                        </ul>
                    </div>

                    <div class="col right">
                        <ul>
                            <li>
                                <h3>
                                    sites
                                </h3>
                            </li>
                            <li>DC</li>
                            <li>MAD Magazine</li>
                            <li>DC Kids</li>
                            <li>DC Universe</li>
                            <li>DC Power Visa</li>
                        </ul>
                    </div>
                </div>
            </div>
        </div>

        <div class="down">
            <div class="container">
                <a href="#" class="btn">sign-up now!</a>
                <ul>
                    <li>
                        <h3>
                            follow us
                        </h3>
                    </li>
                    <li>
                        <i class="fa-brands fa-facebook"></i>
                    </li>
                    <li>
                        <i class="fa-brands fa-square-twitter"></i>
                    </li>
                    <li>
                        <i class="fa-brands fa-youtube"></i>
                    </li>
                    <li>
                        <i class="fa-brands fa-pinterest"></i>
                    </li>
                    <li>
                        <i class="fa-solid fa-location-dot"></i>
                    </li>
                </ul>
            </div>
        </div>

    </footer>
</template>

<style scoped lang="scss">
@use "../style/partials/variables" as *;
@use "../style/partials/mixins" as *;

footer {
    .up {
        height: 320px;
        background-image: url(../assets/img/footer-bg.jpg);
        background-size: cover;
        .container {
            position: relative;
            img {
                width: 500px;
                position: absolute;
                top: -90px;
                right: 0;
            }
            .row {
                display: flex;
                .col {
                    width: 150px;
                    li {
                        font-size: .7rem;
                        color: grey;
                        margin-bottom: .5rem;
                        cursor: pointer;
                    }
                    h3 {
                        font-size: .8rem;
                        text-transform: uppercase;
                        color: white;
                        margin: 1rem 0;
                        cursor: default;
                    }
                }

            }
        }
    }

    .down {
        position: relative;
        z-index: 1;
        height: 100px;
        background-color: #303030;
        .container {
            @include flex(space-between, center);
            // display: flex;
            // justify-content: space-between;
            // align-items: center;
            a.btn {
                text-transform: uppercase;
                color: white;
                border: 2px solid $primary;
                padding: 15px;
            }
            ul {
                display: flex;
                align-items: center;
                gap: 1rem;
                i {
                    font-size: 30px;
                    filter: invert(50%);
                    cursor: pointer;
                }
            }
            h3 {
                color: $primary;
                text-transform: uppercase;
            }
        }
    }
}
</style>