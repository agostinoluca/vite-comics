
<script>
export default {
    name: 'AppHeader'
}
</script>

<template>
    <header>
        <div class="container">
            <div class="row p-2 justify-content-between align-items-center">
                <div class="d-flex align-items-center">
                    <img src="../assets/img/logo.png" alt="logo DC">
                </div>
                <!-- /.div for Logo image -->
                <nav>
                    <ul class="d-flex g-2">
                        <li><a href="#">CHARACTERS</a></li>
                        <li><a href="#">COMICS</a></li>
                        <li><a href="#">MOVIES</a></li>
                        <li><a href="#">TV</a></li>
                        <li><a href="#">GAMES</a></li>
                        <li><a href="#">COLLECTIBLES</a></li>
                        <li><a href="#">VIDEOS</a></li>
                        <li><a href="#">FANS</a></li>
                        <li><a href="#">NEWS</a></li>
                        <li><a href="#">SHOP</a></li>
                    </ul>
                </nav>
                <!-- /nav menù Header -->
            </div>
        </div>
    </header>
    <!-- /header -->
</template>

<style scoped>
a {
    color: var(--dc-dark);
    font-size: 0.75rem;
    font-weight: 600;
}
</style>