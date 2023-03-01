<script>
export default {

}
</script>

<template>
    <header class="main-header">

        <div class="header container">

            <nav class="nav-row">

                <div class="col-img">

                    <img src="/images/dc-logo.png" alt="">

                </div>

                <ul class="col-4 list-row">

                    <li class="nav-list__item">

                        <a href="">characters</a>

                    </li>

                    <li class="nav-list__item active">

                        <a href="" class="active">comics</a>

                    </li>

                    <li class="nav-list__item">

                        <a href="">movies</a>

                    </li>

                    <li class="nav-list__item">

                        <a href="">tv</a>

                    </li>

                    <li class="nav-list__item">

                        <a href="">games</a>

                    </li>

                    <li class="nav-list__item">

                        <a href="">collectibles</a>

                    </li>

                    <li class="nav-list__item">

                        <a href="">videos</a>

                    </li>

                    <li class="nav-list__item">

                        <a href="">fans</a>

                    </li>

                    <li class="nav-list__item">

                        <a href="">news</a>

                    </li>

                    <li class="nav-list__item">

                        <a href="">shop</a>

                    </li>

                </ul>

            </nav>

        </div>

    </header>
</template>

<style lang="scss" scoped>
@use '../style/partials/reset' as *;
@use '../style/partials/variables' as *;

.header {
    padding: 1.5rem 2rem;
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