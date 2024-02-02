<script>
export default {
    name: 'AppMain',
}
</script>

<template>
    <main>
        <div class="top_main">
            <div class="container p-3">
                <h1>Content goes here</h1>
            </div>
        </div>
        <div class="bottom_main">
            <div class="container d-flex justify-content-center p-3">
                <div class="row">
                    <div class="icon_nav">
                        <div>
                            <img src="../assets/img/digital-comics.png" alt="Digital Comics">
                        </div>
                        <div>
                            <p>DIGITAL COMICS</p>
                        </div>
                    </div>
                    <div class="icon_nav">
                        <div>
                            <img src="../assets/img/merchandise.png" alt="Digital Comics">
                        </div>
                        <div>
                            <p>DC MERCHANDISE</p>
                        </div>
                    </div>
                    <div class="icon_nav">
                        <div>
                            <img src="../assets/img/subscriptions.png" alt="Digital Comics">
                        </div>
                        <div>
                            <p>DIGITAL COMICS</p>
                        </div>
                    </div>
                    <div class="icon_nav">
                        <div>
                            <img src="../assets/img/shop-locator.png" alt="Digital Comics">
                        </div>
                        <div>
                            <p>DIGITAL COMICS</p>
                        </div>
                    </div>
                    <div class="icon_nav">
                        <div>
                            <img width="100" src="../assets/img/visa.svg" alt="Digital Comics">
                        </div>
                        <div>
                            <p>DIGITAL COMICS</p>
                        </div>
                    </div>
                </div>
            </div>
        </div>

    </main>
</template>

<style scoped>
h1 {
    color: var(--dc-light);
}

.top_main {
    background-color: var(--dc-dark);
}

.bottom_main {
    background-color: var(--dc-primary);
    color: var(--dc-light);

    & .icon_nav {
        width: calc((100% / 5) - 2rem);
        display: flex;
        align-items: center;
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