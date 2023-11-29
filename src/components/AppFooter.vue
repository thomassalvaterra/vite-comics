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
                        <li><a href="#">Characters</a></li>
                        <li><a href="#">Comics</a></li>
                        <li><a href="#">Movies</a></li>
                        <li><a href="#">TV</a></li>
                        <li><a href="#">Games</a></li>
                        <li><a href="#">Videos</a></li>
                        <li><a href="#">News</a></li>
                        <br>
                    </ul>
                    <div class="title"><strong>SHOP</strong></div>
                    <ul>
                        <li><a href="#">Shop DC</a></li>
                        <li><a href="#">Shop DC Collectibles</a></li>
                    </ul>
                </div>
                <div class="list">
                    <div class="title"><strong>DC</strong></div>
                    <ul>
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
                        <li><a href="#">Contact us</a></li>
                    </ul>
                </div>
                <div class="list">
                    <div class="title"><strong>SITES</strong></div>
                    <ul>
                        <li><a href="#">DC</a></li>
                        <li><a href="#">MAD Magazine</a></li>
                        <li><a href="#">DC Kids</a></li>
                        <li><a href="#">DC Universe</a></li>
                        <li><a href="#">DC Power Visa</a></li>
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
    font-size: 13px;
    line-height: 20px;
}

li a {
    text-decoration: none;
    color: rgb(127, 127, 129);
}

li :hover {
    color: white;
}
</style>