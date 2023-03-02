<script>
import FooterMenus from './FooterMenus.vue';
export default {
    components: {
        FooterMenus
    },

    data() {
        return {
            footerMenuDcComics: {
                title: 'dc comics',
                links: [
                    'Characters',
                    'Comics',
                    'Movies',
                    'TV',
                    'Games',
                    'Videos',
                    'News'
                ]
            },
            footerMenuShop: {
                title: 'shop',
                links: [
                    'Shop DC',
                    'Shop DC Collectibles'
                ]
            },
            footerMenuDc: {
                title: 'dc',
                links: [
                    'Terms of Use',
                    'Privacy policy (New)',
                    'Ad Choices',
                    'Advertising',
                    'Jobs',
                    'Subscriptions',
                    'Talent Workshops',
                    'CPSC Certificates',
                    'Ratings',
                    'Shop Help',
                    'Contact Us'
                ]
            },
            footerMenuSites: {
                title: 'sites',
                links: [
                    'DC',
                    'MAD Magazine',
                    'DC Kids',
                    'DC Universe Online (Best MMO-RPG Ever)',
                    'DC Power Visa'
                ]
            },

        }
    }
}
</script>

<template>
    <footer>

        <div class="main-footer">

            <div class="footer container">

                <img class="footer-logo" src="/images/dc-logo-bg.png" alt="">

                <div class="row">

                    <div class="col row-column">

                        <FooterMenus :title="footerMenuDcComics.title" :links="footerMenuDcComics.links" />

                        <FooterMenus :title="footerMenuShop.title" :links="footerMenuShop.links" />

                    </div>

                    <div class="col">

                        <FooterMenus :title="footerMenuDc.title" :links="footerMenuDc.links" />

                    </div>

                    <div class="col">

                        <FooterMenus :title="footerMenuSites.title" :links="footerMenuSites.links" />

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