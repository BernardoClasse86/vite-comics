<script>
export default {

}
</script>

<template>
    <footer>

        <div class="main-footer">

            <div class="footer container">

                <img class="footer-logo" src="/images/dc-logo-bg.png" alt="">

                <div class="row">

                    <div class="col row-column">

                        <div>

                            <h2 class="footer-item__title">dc comics</h2>

                            <ul>
                                <li class="footer-item__text">Characters</li>
                                <li class="footer-item__text">Comics</li>
                                <li class="footer-item__text">Movies</li>
                                <li class="footer-item__text">TV</li>
                                <li class="footer-item__text">Games</li>
                                <li class="footer-item__text">Videos</li>
                                <li class="footer-item__text">News</li>
                            </ul>

                        </div>

                        <div>

                            <h2 class="footer-item__title">shop</h2>

                            <ul>
                                <li class="footer-item__text">Shop DC</li>
                                <li class="footer-item__text">Shop DC Collectibles</li>
                            </ul>
                        </div>

                    </div>

                    <div class="col">

                        <h2 class="footer-item__title">dc</h2>

                        <ul>
                            <li class="footer-item__text">Terms of Use</li>
                            <li class="footer-item__text">Privacy policy (New)</li>
                            <li class="footer-item__text">Ad Choices</li>
                            <li class="footer-item__text">Advertising</li>
                            <li class="footer-item__text">Jobs</li>
                            <li class="footer-item__text">Subscriptions</li>
                            <li class="footer-item__text">Talent Workshops</li>
                            <li class="footer-item__text">CPSC Certificates</li>
                            <li class="footer-item__text">Ratings</li>
                            <li class="footer-item__text">Shop Help</li>
                            <li class="footer-item__text">Contact Us</li>
                        </ul>

                    </div>

                    <div class="col">

                        <h2 class="footer-item__title">sites</h2>

                        <ul>
                            <li class="footer-item__text">DC</li>
                            <li class="footer-item__text">MAD Magazine</li>
                            <li class="footer-item__text">DC Kids</li>
                            <li class="footer-item__text">DC Universe Online (Best MMO-RPG Ever)</li>
                            <li class="footer-item__text">DC Power Visa</li>
                        </ul>

                    </div>

                </div>

            </div>

        </div>

        <div class="second-footer-bg">

            <div class="links container">

                <div class="row-links">

                    <div>
                        <button class="sing-up-btn">sing-up now!</button>
                    </div>

                    <div class="row-social">

                        <h1 class="social__title">follow us</h1>

                        <ul class="row-social-links">
                            <li>
                                <a href=""><img src="/images/footer-facebook.png" alt=""></a>
                            </li>

                            <li>
                                <a href=""><img src="/images/footer-twitter.png" alt=""></a>
                            </li>

                            <li>
                                <a href=""><img src="/images/footer-youtube.png" alt=""></a>
                            </li>

                            <li>
                                <a href=""><img src="/images/footer-pinterest.png" alt=""></a>
                            </li>

                            <li>
                                <a href=""><img src="/images/footer-periscope.png" alt=""></a>
                            </li>

                        </ul>

                    </div>

                </div>

            </div>

        </div>

    </footer>
</template>

<style lang="scss" scoped>
@use '../style/partials/reset' as *;
@use '../style/partials/variables' as *;

//// MAIN FOOTER ////

.main-footer {
    background-image: url(/images/footer-bg.jpg);
    background-size: cover;
    background-position: center;
    background-repeat: no-repeat;
}

// FIRST FOOTER //
.footer {
    padding: 2.5rem 2rem;
    position: relative;
}

.footer-logo {
    position: absolute;
    right: 0;
    top: 50%;
    transform: translateY(-50%);
    z-index: 1;
}

.row {
    display: flex;
    gap: 1.5rem;
}

.row-column {
    display: flex;
    flex-direction: column;
    gap: 1.5rem;
}

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

// /FIRST FOOTER //

// SECOND FOOTER //

.second-footer-bg {
    background-color: $footer-lnk-bar;
    position: relative;
    z-index: 2;
}

.links {
    padding: 1.75rem 2.5rem;
}

.row-links {
    display: flex;
    align-items: center;
    justify-content: space-between;
}

.sing-up-btn {
    padding: 1rem;
    color: white;
    font-size: 1rem;
    border: 2px solid #0282F9;
    text-transform: uppercase;
    cursor: pointer;
}

.row-social {
    display: flex;
    align-items: center;
    gap: 1.75rem;
}

.row-social-links {
    display: flex;
    align-items: center;
    gap: 1rem;
}

.social__title {
    text-transform: uppercase;
    color: #0282F9;
    font-size: 1rem;
}

// /SECOND FOOTER //

//// /MAIN FOOTER ////
</style>