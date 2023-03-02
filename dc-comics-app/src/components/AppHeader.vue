<script>
import HeaderNav from './HeaderNav.vue';
import Logo from './Logo.vue'
export default {
    components: {
        Logo,
        HeaderNav
    },

    data() {
        return {
            navMenu: {
                links: [
                    'characters',
                    'comics',
                    'movies',
                    'tv',
                    'games',
                    'collectibles',
                    'video',
                    'fans',
                    'news',
                    'shop'
                ]
            }
        }
    }

}
</script>

<template>
    <header class="main-header">

        <div class="header container">

            <nav class="nav-row">

                <Logo />

                <HeaderNav :links="navMenu.links" />

            </nav>

        </div>

    </header>
</template>

<style lang="scss" scoped>
@use '../style/partials/reset' as *;
@use '../style/partials/variables' as *;

.header {
    padding: 1rem 2rem;
}

.nav-row {
    display: flex;
    justify-content: space-between;
    align-items: center;

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
}
</style>