<script>
export default {
    name: "AppFunzionalita",
    data() {
        return {
            icon: [
                {
                    text: "DIGITAL COMICS",
                    url: "#digitalComics",
                    src: "buy-comics-digital-comics.png"
                },
                {
                    text: "DC MERCHANDISE",
                    url: "#merchandise"
                },
                {
                    text: "SUBSCRIPTION",
                    url: "#sub"
                },
                {
                    text: "COMIC SHOP LOCATOR",
                    url: "#comicShop"
                },
                {
                    text: "DC POWER VISA",
                    url: "#powerVisa"
                }
            ]
        }
    },
    mounted() {
        console.log("AppFunzionalita Caricato");
    }
}
</script>

<template>
    <section>
        <div class="container">
            <nav v-for="prodotto in icon">
                <img :src="prodotto.src" alt="">
                <a href="prodotto.url">{{ prodotto.text }}</a>
            </nav>
        </div>
    </section>
</template>

<style scoped>
section {
    background-color: rgb(52, 161, 235);
    color: white;
}

.container {
    height: 150px;
    display: flex;
    align-items: center;
    justify-content: space-around;
    width: 1400px;
    margin: 0 auto;
}

nav a {
    text-decoration: none;
    color: white;
}
</style>