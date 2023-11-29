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
        <img src="../assets/img/dc-logo.png" alt="DC Logo">
        <nav>
            <a v-for="categories in menu" href="categories.url"><strong>{{ categories.text }}</strong></a>
        </nav>
    </header>
</template>

<style scoped>
header {
    margin: 40px auto;
    width: 1400px;
    display: flex;
    justify-content: space-between;
    align-items: center;
    height: 3rem;
}

nav a {
    margin: 0 1rem;
    text-decoration: none;
    color: #222;
    font-size: 14px;
}

a :hover {
    border-bottom: 2px solid rgb(52, 161, 235);
}
</style>
