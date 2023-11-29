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
        <div class="footerLinks">

        </div>
        <div class="bgLogo">

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
    width: 1400px;
}

.bgLogo {
    width: 40%;
    background-size: cover;
    background-position: center;
    background-image: url("../assets/img/dc-logo-bg.png");
}

footer {
    background-color: rgb(70, 70, 70);
    height: 134px;
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
</style>