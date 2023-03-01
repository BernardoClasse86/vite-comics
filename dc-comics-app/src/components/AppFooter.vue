<script>
export default {

}
</script>

<template>
    <!-- merch -->
    <section>

        <div class="merch-outro">

            <div class="merch-container">

                <ul class="merch-row">

                    <li class="merch__item">

                        <img class="merch-item__thumb" src="/images/buy-comics-digital-comics.png" alt="">
                        <p class="merch-item__text">digital comics</p>

                    </li>

                    <li class="merch__item">

                        <img class="merch-item__thumb" src="/images/buy-comics-merchandise.png" alt="">
                        <p class="merch-item__text">dc merchandise</p>

                    </li>

                    <li class="merch__item">

                        <img class="merch-item__thumb" src="/images/buy-comics-shop-locator.png" alt="">
                        <p class="merch-item__text">subscription</p>

                    </li>

                    <li class="merch__item">

                        <img class="merch-item__thumb" src="/images/buy-comics-subscriptions.png" alt="">
                        <p class="merch-item__text">comic store locator</p>

                    </li>

                    <li class="merch__item">

                        <!-- <img src="/images/buy-dc-power-visa.svg" alt="">  not working -->
                        <img class="merch-item__thumb" src="/images/buy-comics-subscriptions.png" alt="">
                        <p class="merch-item__text">dc power visa</p>

                    </li>

                </ul>

            </div>

        </div>

    </section>
    <!-- /merch -->

    <section>
        <footer class="main-footer">
            <div class="footer-content"></div>
        </footer>
    </section>
</template>

<style lang="scss" scoped>
.merch-outro {
    background-color: #0282F9;
}

.merch-container {
    max-width: 1400px;
    margin: 0 auto;
    padding: 3rem 5rem;
}

.merch-row {
    display: flex;
    justify-content: space-between;
    gap: 2rem;
}

.merch__item {
    display: flex;
    align-items: center;
    gap: 0.5rem;

    .merch-item__thumb {
        aspect-ratio: 1;
        width: 4rem;
        object-fit: contain;
        object-position: center;
    }

    .merch-item__text {
        color: white;
        cursor: pointer;
        text-transform: uppercase;
    }
}
</style>