<script>
export default {
    name: "AppHeader",
    data() {
        return {
            menu: [
                {
                    text: "CHARACTERS",
                    url: "#characters"
                },
                {
                    text: "COMICS",
                    url: "#comics"
                },
                {
                    text: "MOVIES",
                    url: "#movies"
                },
                {
                    text: "TV",
                    url: "#tv"
                },
                {
                    text: "GAMES",
                    url: "#games"
                },
                {
                    text: "COLLECTIBLES",
                    url: "#collectibles"
                },
                {
                    text: "VIDEOS",
                    url: "#videos"
                },
                {
                    text: "FANS",
                    url: "#fans"
                },
                {
                    text: "NEWS",
                    url: "#news"
                },
                {
                    text: "SHOP",
                    url: "#shop"
                }
            ]
        }
    },
    mounted() {
        console.log("AppHeader Caricato");
    }
}
</script>

<template>
    <header>
        <nav>
            <img src="../assets/img/dc-logo.png" alt="DC Logo">
            <a v-for="categories in menu" href="categories.url">{{ categories.text }}</a>
        </nav>
    </header>
</template>

<style scoped>
header {
    margin: 40px auto;
    width: 1400px;
}

nav {
    display: flex;
    justify-content: space-between;
    align-items: center;
}

nav a {
    margin: 0 1rem;
    text-decoration: none;
    color: #222;
}
</style>
