<script>
import ComicsCard from "./ComicsCard.vue";
export default {
    name: 'AppMain',
    components: {
        ComicsCard
    },
    data() {
        return {
            comics: [
                {
                    "thumb": "https://www.coverbrowser.com/image/action-comics/1-1.jpg",
                    "price": "$19.99",
                    "series": "Action Comics",
                    "type": "comic book"
                },
                {
                    "thumb": "https://www.panini.it/media/catalog/product/cache/a5b5dd3adfe0d321084804c738f29601/M/1/M1BLLA015ISBN_0.jpg",
                    "price": "$3.99",
                    "series": "American Vampire 1976",
                    "type": "comic book"
                },
                {
                    "thumb": "https://media.wired.com/photos/593384dad80dd005b42b2817/master/w_2560%2Cc_limit/Aquaman-16.jpg",
                    "price": "$16.99",
                    "series": "Aquaman",
                    "type": "graphic novel"
                },
                {
                    "thumb": "https://d29xot63vimef3.cloudfront.net/image/batgirl/1-1.jpg",
                    "price": "$2.99",
                    "series": "Batgirl",
                    "type": "comic book"
                },
                {
                    "thumb": "https://static.posters.cz/image/750/locandine-film-in-plexiglass-batman-prowl-comic-cover-i69653.jpg",
                    "price": "$3.99",
                    "series": "Batman",
                    "type": "comic book"
                },
                {
                    "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/5/50/Batman_Beyond_v.1_1.jpg",
                    "price": "$2.99",
                    "series": "Batman Beyond",
                    "type": "comic book"
                },
                {
                    "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/0/0d/Batman_Superman_Vol_1_1.jpg",
                    "price": "$3.99",
                    "series": "Batman/Superman",
                    "type": "comic book"
                },
                {
                    "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/c/cf/Batman_Superman_Annual_Vol_2_1.jpg",
                    "price": "$4.99",
                    "series": "Batman/Superman Annual",
                    "type": "comic book"
                },
                {
                    "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/5/54/Batman_The_Joker_War_Zone_Vol_1_1.jpg",
                    "price": "$5.99",
                    "series": "Batman: The Joker War Zone",
                    "type": "comic book"
                },
                {
                    "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/6/64/Batman_Three_Jokers_Collected.jpg",
                    "price": "$6.99",
                    "series": "Batman: Three Jokers",
                    "type": "comic book"
                },
                {
                    "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/f/f8/Batman_White_Knight_Presents_Harley_Quinn_Vol_1_1.jpg",
                    "price": "$4.99",
                    "series": "Batman: White Knight Presents: Harley Quinn",
                    "type": "comic book"
                },
                {
                    "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/c/c8/Catwoman_Vol_2_1.jpg",
                    "price": "$16.99",
                    "series": "Catwoman",
                    "type": "graphic novel"
                }
            ]
        }

    }
}
</script>

<template>
    <main>
        <div class="top_main">
            <div class="jumbotron">

            </div>
            <div class="container p-3">
                <h3>CURRENT SERIES</h3>
                <div class="row">
                    <div class="col-2" v-for="comic in comics">
                        <ComicsCard :comic="comic"></ComicsCard>
                    </div>
                </div>
            </div>
        </div>
        <!-- /.top_main -->

        <div class="bottom_main">
            <div class="container p-3">
                <div class="row">
                    <div class="icon_nav">
                        <div>
                            <img src="../assets/img/digital-comics.png" alt="Digital Comics">
                        </div>
                        <div>
                            <span>DIGITAL COMICS</span>
                        </div>
                    </div>
                    <!-- /.icon_nav DIGITAL COMICS -->

                    <div class="icon_nav">
                        <div>
                            <img src="../assets/img/merchandise.png" alt="Digital Comics">
                        </div>
                        <div>
                            <span>DC MERCHANDISE</span>
                        </div>
                    </div>
                    <!-- /.icon_nav DC MERCHANDISE -->

                    <div class="icon_nav">
                        <div>
                            <img src="../assets/img/subscriptions.png" alt="Digital Comics">
                        </div>
                        <div>
                            <span>SUBSCRIPTION</span>
                        </div>
                    </div>
                    <!-- /.icon_nav SUBSCRIPTION -->

                    <div class="icon_nav">
                        <div>
                            <img src="../assets/img/shop-locator.png" alt="Digital Comics">
                        </div>
                        <div>
                            <span>COMIC SHOP LOCATOR</span>
                        </div>
                    </div>
                    <!-- /.icon_nav COMIC SHOP LOCATOR -->

                    <div class="icon_nav">
                        <div>
                            <img width="100" src="../assets/img/visa.svg" alt="Digital Comics">
                        </div>
                        <div>
                            <span>DC POWER VISA</span>
                        </div>
                    </div>
                    <!-- /.icon_nav DC POWER VISA -->

                </div>
            </div>
        </div>
        <!-- /.bottom_main -->

    </main>
</template>

<style scoped>
.top_main {
    background-color: var(--dc-dark);

    & .jumbotron {
        background-image: url(../assets/img/jumbotron.jpg);
        background-size: cover;
        height: 18rem;
    }

    & h3 {
        display: inline-flex;
        color: var(--dc-light);
        background-color: var(--dc-primary);
        padding: 1rem;
    }
}

.bottom_main {
    background-color: var(--dc-primary);
    color: var(--dc-light);

    & .icon_nav {
        width: calc((100% / 5) - 2rem);
        display: flex;
        align-items: center;
        justify-content: center;
        gap: 0.5rem;
        margin: 1rem;
        cursor: pointer;
    }

    & span {
        font-size: 0.75rem;
    }

    & img {
        max-height: 4rem;
    }
}
</style>