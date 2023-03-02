<script>
export default {
    props: {
        title: String,
        links: Array
    }
}
</script>

<template>
    <div>

        <h2 class="footer-item__title">{{ title }}</h2>

        <ul>
            <li class="footer-item__text" v-for="(link, i) in links">{{ link }}</li>
        </ul>

    </div>
</template>

<style lang="scss" scoped>
@use '../style/partials/variables' as *;

.footer-item__title {
    color: white;
    font-weight: bold;
    text-transform: uppercase;
    font-size: 1rem;
    margin-bottom: 1.25rem;
}

.footer-item__text {
    color: $footer-text;
    font-size: 0.75rem;
    margin-bottom: 0.5rem;
    cursor: pointer;
}
</style>