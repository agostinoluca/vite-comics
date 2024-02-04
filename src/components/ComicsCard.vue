
<script>
export default {
    name: 'ComicsCard',
    props: {
        comic: Object
    }
}
</script>

<template>
    <div class="card p-1">
        <img :src="comic.thumb" alt="">
        <h5>{{ comic.series }}</h5>
    </div>
</template>


<style scoped>
.card {
    color: var(--dc-light);
}

.card img {
    width: 100%;
    aspect-ratio: 1;
    object-fit: cover;
    object-position: top;
}
</style>