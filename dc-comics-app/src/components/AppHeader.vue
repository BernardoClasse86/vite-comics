<script>
export default {

}
</script>

<template>
    <header class="main-header">

        <div class="header-container">

            <nav class="nav-row">

                <div class="col-img">

                    <img src="/images/dc-logo.png" alt="">

                </div>

                <ul class="col-4 list-row">

                    <li class="nav-list__item">characters</li>
                    <li class="nav-list__item active">comics</li>
                    <li class="nav-list__item">movies</li>
                    <li class="nav-list__item">tv</li>
                    <li class="nav-list__item">games</li>
                    <li class="nav-list__item">collectibles</li>
                    <li class="nav-list__item">videos</li>
                    <li class="nav-list__item">fans</li>
                    <li class="nav-list__item">news</li>
                    <li class="nav-list__item">shop</li>

                </ul>

            </nav>

        </div>

    </header>
</template>

<style lang="scss" scoped>
@use '../style/partials/reset';
@use '../style/partials/variables';

.header-container {
    max-width: 1400px;
    margin: 0 auto;
    padding: 1.5rem 1rem;
}

.nav-row {
    display: flex;
    justify-content: space-between;
    align-items: center;
}

.col-img {
    flex-shrink: 0;
}

.list-row {
    display: flex;
}

.nav-list__item {
    line-height: 1.5rem;
    padding: 0 1rem;
    font-size: 0.80rem;
    font-weight: bold;
    text-transform: uppercase;
    cursor: pointer;

    &.active,
    &:hover {
        color: #0282F9;
    }

    &.active::after {
        content: '';
        display: block;
        width: 100%;
        height: 0.25rem;
        background-color: #0282F9;
    }
}
</style>