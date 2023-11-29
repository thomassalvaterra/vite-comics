<script>
export default {
    name: "AppFooter",
    data() {
        return {
            image: [
                {
                    src: "/src/assets/img/footer-facebook.png"
                },
                {
                    src: "/src/assets/img/footer-periscope.png"
                },
                {
                    src: "/src/assets/img/footer-pinterest.png"
                },
                {
                    src: "/src/assets/img/footer-twitter.png"
                },
                {
                    src: "/src/assets/img/footer-youtube.png"
                }
            ]
        }
    },
}
</script>

<template>
    <div class="murales">
        <div class="container">
            <div class="footerLinks">
                <div class="list">
                    <div class="title"><strong>DC COMICS</strong></div>
                    <ul>
                        <li>Characters</li>
                        <li>Comics</li>
                        <li>Movies</li>
                        <li>TV</li>
                        <li>Games</li>
                        <li>Videos</li>
                        <li>News</li>
                        <br>
                    </ul>
                    <div class="title"><strong>SHOP</strong></div>
                    <ul>
                        <li>Shop DC</li>
                        <li>Shop DC Collectibles</li>
                    </ul>
                </div>
                <div class="list">
                    <div class="title"><strong>DC</strong></div>
                    <ul>
                        <li>Terms Of Use</li>
                        <li>Privacy policy (New)</li>
                        <li>Ad Choices</li>
                        <li>Advertising</li>
                        <li>Jobs</li>
                        <li>Subscriptions</li>
                        <li>Talent Workshops</li>
                        <li>CPSC Certificates</li>
                        <li>Ratings</li>
                        <li>Shop Help</li>
                        <li>Contact us</li>
                    </ul>
                </div>
                <div class="list">
                    <div class="title"><strong>SITES</strong></div>
                    <ul>
                        <li>DC</li>
                        <li>MAD Magazine</li>
                        <li>DC Kids</li>
                        <li>DC Universe</li>
                        <li>DC Power Visa</li>
                    </ul>
                </div>



            </div>
            <div class="bgLogo">

            </div>
        </div>
    </div>

    <footer>
        <div class="container">
            <button id="btn"><b>SIGN-UP NOW!</b></button>
            <div class="pages">
                <span id="mr"><strong>FOLLOW US</strong></span>
                <nav v-for="img in image">
                    <img :src="img.src" class="space">
                </nav>
            </div>
        </div>
    </footer>
</template>
<style scoped>
.murales {
    display: flex;
    padding: 0 10%;
    height: 20rem;
    background-image: url("../assets/img/footer-bg.jpg");
    background-size: cover;
}

.footerLinks {
    display: flex;
    margin-top: 20px;
}

.bgLogo {
    width: 40%;
    background-size: cover;
    background-position: center;
    background-image: url("../assets/img/dc-logo-bg.png");
}

footer {
    background-color: rgb(70, 70, 70);
    height: 6rem;
    display: flex;
}

.container {
    width: 1400px;
    margin: 0 auto;
    display: flex;
    justify-content: space-between;
    align-items: center;
}

#btn {
    border: 3px solid rgb(52, 161, 235);
    background-color: rgb(70, 70, 70);
    color: white;
    padding: 20px;
    font-size: 18px;
}

.pages {
    display: flex;
    align-items: center;
}

#mr {
    margin-right: 20px;
    color: rgb(52, 161, 235);
    font-size: 20px;
}

.space {
    margin: 10px;
}

.title {
    color: whitesmoke;
    margin-bottom: 20px;
    font-size: 20px;
}

.list {
    margin-right: 25px;
}

ul {
    color: white;
}

li {
    list-style-type: none;
    color: rgb(127, 127, 129);
    font-size: 13px;
    line-height: 20px;
}
</style>