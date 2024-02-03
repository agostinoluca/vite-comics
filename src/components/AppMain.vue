<script>
export default {
    name: 'AppMain',
}
</script>

<template>
    <main>
        <div class="top_main">
            <div class="jumbotron">

            </div>
            <div class="container p-3">
                <h1>Content goes here</h1>
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
                            <p>DIGITAL COMICS</p>
                        </div>
                    </div>
                    <!-- /.icon_nav DIGITAL COMICS -->

                    <div class="icon_nav">
                        <div>
                            <img src="../assets/img/merchandise.png" alt="Digital Comics">
                        </div>
                        <div>
                            <p>DC MERCHANDISE</p>
                        </div>
                    </div>
                    <!-- /.icon_nav DC MERCHANDISE -->

                    <div class="icon_nav">
                        <div>
                            <img src="../assets/img/subscriptions.png" alt="Digital Comics">
                        </div>
                        <div>
                            <p>SUBSCRIPTION</p>
                        </div>
                    </div>
                    <!-- /.icon_nav SUBSCRIPTION -->

                    <div class="icon_nav">
                        <div>
                            <img src="../assets/img/shop-locator.png" alt="Digital Comics">
                        </div>
                        <div>
                            <p>COMIC SHOP LOCATOR</p>
                        </div>
                    </div>
                    <!-- /.icon_nav COMIC SHOP LOCATOR -->

                    <div class="icon_nav">
                        <div>
                            <img width="100" src="../assets/img/visa.svg" alt="Digital Comics">
                        </div>
                        <div>
                            <p>DC POWER VISA</p>
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
h1 {
    color: var(--dc-light);
}

.top_main {
    background-color: var(--dc-dark);

    & .jumbotron {
        background-image: url(../assets/img/jumbotron.jpg);
        background-size: cover;
        height: 18rem;
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

    & p {
        font-size: 0.75rem;
    }

    & img {
        max-height: 4rem;
    }
}
</style>