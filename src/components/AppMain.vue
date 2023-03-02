<script>
import Comics from './Comics.vue'
export default {

    components: {

        Comics
    },

    data() {
        return {

            comics: [
                {
                    thumb: "https://www.syfy.com/sites/syfy/files/2021/11/action_comics_1037_cover.jpg",
                    price: "$19.99",
                    series: "Action Comics",
                    type: "comic book"
                },
                {
                    thumb: "https://www.panini.it/media/catalog/product/cache/a5b5dd3adfe0d321084804c738f29601/M/1/M1BLLA015ISBN_0.jpg",
                    price: "$3.99",
                    series: "American Vampire 1976",
                    type: "comic book"
                },
                {
                    thumb: "https://www.washingtonpost.com/wp-apps/imrs.php?src=http://www.washingtonpost.com/news/comic-riffs/wp-content/uploads/sites/15/2017/06/AQM_Cv25_ds.jpg&w=1440",
                    price: "$16.99",
                    series: "Aquaman",
                    type: "graphic novel"
                },
                {
                    thumb: "https://cdn.nexternal.com/dreamland/images/batgirl_1B.jpg",
                    price: "$2.99",
                    series: "Batgirl",
                    type: "comic book"
                },
                {
                    thumb: "https://cdn.nexternal.com/dreamland/images/bat52_2leenm.jpg",
                    price: "$3.99",
                    series: "Batman",
                    type: "comic book"
                },
                {
                    thumb: "https://i.pinimg.com/474x/16/11/46/16114656b94c5b250891dc583fdffbc1.jpg",
                    price: "$2.99",
                    series: "Batman Dark Knights Metal",
                    type: "comic book"
                },
                {
                    thumb: "https://media.forbiddenplanet.com/products/diamond/lunar/0122DC011.jpg",
                    price: "$3.99",
                    series: "Batman/Superman",
                    type: "comic book"
                },
                {
                    thumb: "https://d1466nnw0ex81e.cloudfront.net/n_iv/600/946145.jpg",
                    price: "$4.99",
                    series: "Batman/Superman Annual",
                    type: "comic book"
                },
                {
                    thumb: "https://m.media-amazon.com/images/I/41nGyVF7C2L.jpg",
                    price: "$5.99",
                    series: "Batman: The Joker War Zone",
                    type: "comic book"
                },
                {
                    thumb: "https://pbs.twimg.com/media/EdKd9M_VAAA5Lm4?format=jpg&name=4096x4096",
                    price: "$6.99",
                    series: "Batman: Three Jokers",
                    type: "comic book"
                },
                {
                    thumb: "https://m.media-amazon.com/images/I/51elRyK2tXS.jpg",
                    price: "$4.99",
                    series: "Batman: White Knight Presents: Harley Quinn",
                    type: "comic book"
                },
                {
                    thumb: "https://s3.amazonaws.com/comicgeeks/comics/covers/large-1806419.jpg?1636800911",
                    price: "$16.99",
                    series: "Catwoman",
                    type: "graphic novel"
                }
            ]
        }
    }

}
</script>

<template>
    <main class="main-content">

        <div class="hero"></div>

        <div class="comics-content">

            <div class="comic-series">current series</div>

            <div class="comics-container">

                <ul class="grid">

                    <Comics v-for="(comic, i) in comics" :key="i" :series="comic.series" :thumb="comic.thumb" />

                </ul>

            </div>

            <div class="main-btn">Load More</div>

        </div>

    </main>
</template>

<style lang="scss" scoped>
@use '../style/partials/reset' as *;
@use '../style/partials/variables' as *;

.main-content {
    background-color: $main-bg-color;
}

.hero {
    background-image: url(/images/jumbotron.jpg);
    background-position: top;
    background-size: cover;
    background-repeat: no-repeat;
    height: 440px;
}

.comics-content {
    padding: 3rem 2rem;
    position: relative;

    .comic-series {
        position: absolute;
        top: -24px;
        left: 160px;
        padding: 0.5rem 2rem;
        background-color: $merch-bar-color;
        color: white;
        text-transform: uppercase;
        font-size: 1.5rem;
        font-weight: bold;
    }

    .comics-container {
        max-width: 1100px;
        margin: 0 auto;
        font-size: 0.75rem;
    }

    .grid {
        display: grid;
        grid-template-columns: repeat(6, 1fr);
        gap: 0.5rem;
    }
}

.main-btn {
    margin-top: 1rem;
    margin-left: 50%;
    transform: translateX(-50%);
    display: inline-block;
    padding: 0.5rem 2rem;
    font-size: 1rem;
    cursor: pointer;
    color: white;
    font-weight: bold;
    background-color: $active-lnk-color;
}
</style>