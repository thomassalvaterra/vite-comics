<script>
export default {
    // props: ["product"]
    props: {
        carta: Object
    }
}
</script>

<template>
    <div class="card">
        <img :src="carta.thumb" alt="">
        <p>{{ carta.series }}</p>
    </div>
</template>

<style scoped>
.card {
    color: white;
    padding: 1rem;
    width: calc(100% / 6);
    margin: 10px 0;
}

img {
    width: 100%;
    margin-bottom: 10px;
}
</style>