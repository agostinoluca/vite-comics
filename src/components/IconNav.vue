<script>
export default {
    name: 'IconNav',
    props: {
        icon: Object
    }
}
</script>

<template>
    <div>
        <img height="50" :src="icon.img" :alt="icon.alt">
    </div>
    <div>
        <span>{{ icon.title }}</span>
    </div>
</template>


<style scoped>
span {
    font-size: 0.75rem;
}

img {
    max-height: 4rem;
}
</style>