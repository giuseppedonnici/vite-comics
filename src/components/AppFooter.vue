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
        height: 400px;
        background-image: url(../assets/img/footer-bg.jpg);
        background-size: cover;
        .container {
            position: relative;
            img {
                width: 550px;
                position: absolute;
                top: -90px;
                right: 0;
            }
        }
    }
}
</style>