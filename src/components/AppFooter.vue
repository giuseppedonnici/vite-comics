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

            </div>
        </div>

    </footer>
</template>

<style scoped lang="scss">
@use "../style/partials/variables";

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
}
</style>