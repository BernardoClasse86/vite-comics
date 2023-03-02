<script>
export default {
    props: {
        series: String,
        thumb: String,
    }
}
</script>

<template>
    <li class="comics-card">

        <img class="comic__thumb" :src="thumb" alt="">

        <h3 class="card__title">{{ series }}</h3>

    </li>
</template>

<style lang="scss" scoped>
.comics-card {
    padding: 0.25rem;

    .comic__thumb {
        aspect-ratio: 0.75;
        object-fit: contain;
        object-position: center;
        margin-bottom: 1rem;
    }

    .card__title {
        text-align: center;
        font-size: 1rem;
        color: white;
        font-weight: bold;
    }
}
</style>
