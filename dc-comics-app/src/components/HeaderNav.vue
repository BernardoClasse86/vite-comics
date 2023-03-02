<script>
export default {
    props: {
        links: Array
    }

}
</script>

<template>
    <ul class="nav-list-row">

        <li v-for="(link, i) in links" :key="i" class="nav-list__item">

            <a href="">{{ link }}</a>

        </li>

    </ul>
</template>

<style lang="scss" scoped>
@use '../style/partials/variables' as *;

.nav-list-row {
    display: flex;
    gap: 1rem;
}

.nav-list__item {
    line-height: 1.5rem;
    font-size: 0.80rem;
    font-weight: bold;
    text-transform: uppercase;
    cursor: pointer;
    position: relative;

    &.active,
    &:hover {
        color: $active-lnk-color;
    }

}

.active::after {
    content: "";
    position: absolute;
    top: 82px;
    right: 0;
    left: 0;
    border-bottom: 4px solid $active-lnk-color;
    height: 0.25rem;
}
</style>