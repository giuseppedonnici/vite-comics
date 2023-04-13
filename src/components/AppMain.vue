<script>
export default {
    name: "AppMain",
    data() {
        return {
            
        }
    }
}
</script>

<template>
    <main>
        <div class="content">
            <div class="container">
            --> Content goes here &lt;--
            </div>
        </div>

        <div class="cta">

        </div>
    </main>
</template>

<style scoped lang="scss">
@use "../style/partials/variables" as *;

main {
    .content {
        line-height: 100px;
        color: white;
        font-size: 2rem;
        font-weight: bold;
        font-stretch: ultra-condensed;
        background-color: black;
        .container {
            width: 60%;
            margin: 0 auto;
        }
    }
    
    .cta {
        background-color: $primary;
        height: 200px;
    }
}
</style>