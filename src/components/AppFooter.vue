<script>

export default (await import('vue')).defineComponent({
    name: "AppFooter",
})

</script>

<template>
    <!-- parte superiore -->
    <section id="up-footer">
        <div class="container">

            <nav>
                <ul id="list-up-footer">
                    <li class="li-up-footer">
                        <div class="li-img">
                            <img src="../assets/img/buy-comics-digital-comics.png" alt="">
                        </div>

                        <a href="#">DIGITAL COMICS</a>
                    </li>

                    <li class="li-up-footer">
                        <div class="li-img">
                            <img src="../assets/img/buy-comics-merchandise.png" alt="">
                        </div>

                        <a href="#">DC MERCHANDISE</a>
                    </li>

                    <li class="li-up-footer">
                        <div class="li-img">
                            <img src="../assets/img/buy-comics-subscriptions.png" alt="">
                        </div>

                        <a href="#">SUBSCRIPTION</a>
                    </li>

                    <li class="li-up-footer">
                        <div class="li-img">
                            <img src="../assets/img/buy-comics-shop-locator.png" alt="">
                        </div>

                        <a href="#">COMIC SHOP LOCATOR</a>
                    </li>

                    <li class="li-up-footer">
                        <div class="li-img">
                            <img src="../assets/img/buy-dc-power-visa.svg" alt="">
                        </div>

                        <a href="#">DC POWER VISA</a>
                    </li>
                </ul>
            </nav>

        </div>
    </section>

    <!-- parte centrale -->
    <section id="central-footer">
        <div class="container">
            <div id="list-central-footer">
                <div>
                    <ul>
                        <h2>DC COMICS</h2>

                        <li>
                            <a href="#">Characters</a>
                        </li>

                        <li>
                            <a href="#">Comics</a>
                        </li>

                        <li>
                            <a href="#">Movies</a>
                        </li>

                        <li>
                            <a href="#">TV</a>
                        </li>

                        <li>
                            <a href="#">Games</a>
                        </li>

                        <li>
                            <a href="#">Videos</a>
                        </li>

                        <li>
                            <a href="#">News</a>
                        </li>

                    </ul>

                    <ul>
                        <h2>SHOP</h2>

                        <li>
                            <a href="#">Shop DC</a>
                        </li>

                        <li>
                            <a href="#">Shop DC Collectibles</a>
                        </li>
                    </ul>
                </div>

                <div>
                    <ul>
                        <h2>DC</h2>

                        <li>
                            <a href="#">Terms of Use</a>
                        </li>

                        <li>
                            <a href="#">Privacy policy (New)</a>
                        </li>

                        <li>
                            <a href="#">Ad Choises</a>
                        </li>

                        <li>
                            <a href="#">Advertising</a>
                        </li>

                        <li>
                            <a href="#">Jobs</a>
                        </li>

                        <li>
                            <a href="#">Subscriptions</a>
                        </li>

                        <li>
                            <a href="#">Talent Workshops</a>
                        </li>

                        <li>
                            <a href="#">CPSC Certificates</a>
                        </li>

                        <li>
                            <a href="#">Ratings</a>
                        </li>

                        <li>
                            <a href="#">Shop Help</a>
                        </li>

                        <li>
                            <a href="#">Contact Us</a>
                        </li>

                    </ul>
                </div>

                <div>
                    <ul>
                        <h2>SITES</h2>

                        <li>
                            <a href="#">DC</a>
                        </li>

                        <li>
                            <a href="#">MAD Magazine</a>
                        </li>

                        <li>
                            <a href="#">DC Kids</a>
                        </li>

                        <li>
                            <a href="#">DC Universe</a>
                        </li>

                        <li>
                            <a href="#">DC Power Visa</a>
                        </li>

                    </ul>
                </div>
            </div>

            <div id="img-central-footer">

            </div>
        </div>
    </section>

    <!-- parte inferiore -->
    <section id="down-footer">
        <div class="container">

            <div id="left-down-footer">
                <button id="my-button">SIGN-UP NOW!</button>
            </div>

            <div id="right-down-footer">
                <h2>FOLLOW US</h2>

                <div class="icons">
                    <div class="img-icon">
                        <img src="../assets/img/footer-facebook.png" alt="facebook">
                    </div>
                    <div class="img-icon">
                        <img src="../assets/img/footer-twitter.png" alt="twitter">
                    </div>
                    <div class="img-icon">
                        <img src="../assets/img/footer-youtube.png" alt="youtube">
                    </div>
                    <div class="img-icon">
                        <img src="../assets/img/footer-pinterest.png" alt="pinterest">
                    </div>
                    <div class="img-icon">
                        <img src="../assets/img/footer-periscope.png" alt="periscope">
                    </div>
                </div>
            </div>

        </div>
    </section>
</template>

<style lang="scss">
@use '../styles/partials/variables.scss' as *;
@use '../styles/partials/mixins.scss' as *;

// regole parte superiore
#up-footer {
    display: flex;
    align-items: center;
    height: 130px;
    background-color: rgb(12, 124, 236);
    color: white;
}

ul {
    list-style: none;
    font-size: 12px;

    li {
        margin-left: 20px;

        a {
            text-decoration: none;
            color: white;
        }

        img {
            width: 40px;
            margin-right: 10px;
        }
    }
}

#list-up-footer {
    @include flex-around;
}

.li-up-footer {
    @include flex-between-center;
}

// regole parte centrale
#central-footer {
    height: 300px;
    background-image: url("../assets/img/footer-bg.jpg");
    color: white;
}

#central-footer>.container {
    @include flex-between-center;
}

#list-central-footer {
    display: flex;
    justify-content: space-between;
    width: 30%;
}

#list-central-footer>div>ul>li {
    margin-left: 0px;
}

#list-central-footer>div>ul>li>a {
    font-weight: lighter;
    color: rgb(153, 153, 153);

}

#img-central-footer {
    width: 50%;
    height: 300px;
    background-image: url('../assets/img/dc-logo-bg.png');
}

// regole parte inferiore
#down-footer {
    height: 100px;
    background-color: rgb(48, 48, 48);
}

#my-button {
    background-color: rgb(48, 48, 48);
    border: 2px solid rgb(12, 124, 236);
    color: white;
    padding: 10px;

    &:hover {
        cursor: pointer;
    }
}

#down-footer>div.container {
    height: 100px;
    display: flex;
    justify-content: space-between;
    align-items: center;
}

#right-down-footer {
    display: flex;
    width: 30%;
    justify-content: space-between;
    color: rgb(12, 124, 236);
}

.icons {
    width: 60%;
    display: flex;
    justify-content: space-between;
}
</style>