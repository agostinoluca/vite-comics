<script>
export default {
    name: 'AppFooter',
}
</script>

<template>
    <footer>
        <div class="top_footer">
            <div class="container">
                <div class="row">
                    <div class="col-6 d-flex p-3 g-4 ">
                        <div>
                            <h4>DC COMICS</h4>
                            <ul>
                                <li><a href="#">Characters</a></li>
                                <li><a href="#">Comics</a></li>
                                <li><a href="#">Movies</a></li>
                                <li><a href="#">TV</a></li>
                                <li><a href="#">Games</a></li>
                                <li><a href="#">Videos</a></li>
                                <li><a href="#">News</a></li>
                            </ul>

                            <h4>SHOP</h4>
                            <ul>
                                <li><a href="#">Shop DC</a></li>
                                <li><a href="#">Shop DC Collectibles</a></li>
                            </ul>
                        </div>

                        <ul>
                            <h4>DC</h4>
                            <li><a href="#">Terms Of Use</a></li>
                            <li><a href="#">Privacy policy (New)</a></li>
                            <li><a href="#">Ad Choices</a></li>
                            <li><a href="#">Advertising</a></li>
                            <li><a href="#">Jobs</a></li>
                            <li><a href="#">Subscriptions</a></li>
                            <li><a href="#">Talent Workshops</a></li>
                            <li><a href="#">CPSC Certificates</a></li>
                            <li><a href="#">Ratings</a></li>
                            <li><a href="#">Shop Help</a></li>
                            <li><a href="#">Contact Us</a></li>
                        </ul>
                        <ul>
                            <h4>SITES</h4>
                            <li><a href="#">DC</a></li>
                            <li><a href="#">MAD Magazine</a></li>
                            <li><a href="#">DC Kids</a></li>
                            <li><a href="#">DC Universe</a></li>
                            <li><a href="#">DC Power Visa</a></li>
                        </ul>
                    </div>
                    <div class="logo_bg col-6"></div>
                </div>

            </div>
        </div>
        <div class="bottom_footer"></div>
    </footer>
</template>



<style scoped>
.top_footer {
    background-image: url(../assets/img/footer-bg.jpg);
    background-size: cover;
    background-repeat: no-repeat;

    & .logo_bg {
        background-image: url(../assets/img/logo-bg.png);
        background-repeat: no-repeat;
        background-size: auto;
        background-position: center;
    }

    & h4 {
        color: var(--dc-light);
        margin: 0.75rem 0;
    }

    & a {
        color: var(--dc-lightgray);
        font-size: 0.75rem;
        font-weight: 700;
    }
}

.bottom_footer {
    background-color: var(--dc-secondary);
}
</style>