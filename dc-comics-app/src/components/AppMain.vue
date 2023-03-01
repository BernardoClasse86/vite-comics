<script>
export default {

}
</script>

<template>
    <main class="main-content">

        <div class="main container">

            <h1 class="main-content-title"> Content goes here </h1>

        </div>

    </main>
</template>

<style lang="scss" scoped>
@use '../style/partials/reset' as *;
@use '../style/partials/variables' as *;

.main-content {
    background-color: black
}

.main {
    padding: 3rem 2rem;

    .main-content-title {
        color: white;
        font-size: 2rem;
    }
}
</style>