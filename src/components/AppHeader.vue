<script>
export default {
    name: "AppHeader",
    data() {
        return {
            links: [
                {
                    text: "CHARACTERS",
                    url: "#",
                    current: false
                },
                {
                    text: "COMICS",
                    url: "#",
                    current: true
                },
                {
                    text: "MOVIES",
                    url: "#",
                    current: false
                },
                {
                    text: "TV",
                    url: "#",
                    current: false
                },
                {
                    text: "GAMES",
                    url: "#",
                    current: false
                },
                {
                    text: "COLLECTIBLES",
                    url: "#",
                    current: false
                },
                {
                    text: "VIDEOS",
                    url: "#",
                    current: false
                },
                {
                    text: "FANS",
                    url: "#",
                    current: false
                },
                {
                    text: "NEWS",
                    url: "#",
                    current: false
                },
                {
                    text: "SHOP",
                    url: "#",
                    current: false
                },
            ]
        }
    }
}
</script>

<template>
    <header>
        <div class="container">
            <div class="nav-bar">
                <img src="../assets/img/dc-logo.png" alt="">
                <ul>
                    <li v-for="link in links" :class="link.current ? 'active' : ''">
                        <a :href="link.url">{{ link.text }}</a>
                    </li>
                </ul>
            </div>
        </div>
    </header>
</template>

<style scoped lang="scss">
@use "../style/partials/variables" as *;
@use "../style/partials/mixins" as *;

header {
    height: 100px;
    background-color: white;
    .nav-bar {
        @include flex(space-between, center);
        // display: flex;
        // justify-content: space-between;
        // align-items: center;
        height: 100%;
    }

    img {
        width: 70px;
    }

    ul {
        display: flex;
        gap: 1.2rem;
        height: 100%;
        font-size: .7rem;
        font-weight: bold;
        font-stretch: ultra-condensed;

        li {
            &.active {
                color: $primary;
                border-bottom: 5px solid $primary;
            }
    
            &:hover {
                color: $primary;
            }
    
            a {
                line-height: 100px;
            }
        }
    }
}
</style>