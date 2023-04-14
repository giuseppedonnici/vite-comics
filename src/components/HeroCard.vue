<script>
export default {
    name: "HeroCard",
    props: {
        image: String,
        title: String
    }
}
</script>

<template>
    <div class="card">
        <img :src="image" alt="">
        <h3>{{ title }}</h3>
    </div>

</template>

<style scoped lang="scss">
  .card {
    width: calc(100% / 6 - 10px);
    margin: 5px;
    margin-bottom: 2rem;
    img {
        width: 100%;
        height: 150px;
        object-fit: cover;
    }
    h3 {
        font-size: .7rem;
        text-transform: uppercase;
        padding-top: .5rem;
    }
  }

</style>