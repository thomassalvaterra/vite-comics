<script>
export default {
    name: "AppFunzionalita",
    data() {
        return {
            icon: [
                {
                    text: "DIGITAL COMICS",
                    url: "#digitalComics",
                    src: "/src/assets/img/buy-comics-digital-comics.png"
                },
                {
                    text: "DC MERCHANDISE",
                    url: "#merchandise",
                    src: "/src/assets/img/buy-comics-merchandise.png"
                },
                {
                    text: "SUBSCRIPTION",
                    url: "#sub",
                    src: "/src/assets/img/buy-comics-shop-locator.png"
                },
                {
                    text: "COMIC SHOP LOCATOR",
                    url: "#comicShop",
                    src: "/src/assets/img/buy-comics-subscriptions.png"
                },
                {
                    text: "DC POWER VISA",
                    url: "#powerVisa",
                    src: "/src/assets/img/buy-dc-power-visa.svg"
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
    height: 7rem;
    display: flex;
    justify-content: space-around;
    align-items: center;
    width: 1400px;
    margin: 0 auto;
}

nav a {
    text-decoration: none;
    color: white;
    font-size: 13px;
}

img {
    max-width: 50px;
    max-height: 50px;
    margin-right: 10px;
}
</style>