<template>
    <footer>
        <div class="footer-top">
            <div class="container">
                <div class="footer-top__items">
                    <a href="#" class="footer-top__item">
                        <img class="footer-top__item-img" src="../assets/img/buy-comics-digital-comics.png">
                        <p>DIGITAL COMINCS</p>
                    </a>
                    <a href="#" class="footer-top__item">
                        <img class="footer-top__item-img" src="../assets/img/buy-comics-merchandise.png">
                        <p>DC MERCHANDISE</p>
                    </a>
                    <a href="#" class="footer-top__item">
                        <img class="footer-top__item-img" src="../assets/img/buy-comics-subscriptions.png">
                        <p>SUBSCRIPTIONS</p>
                    </a>
                    <a href="#" class="footer-top__item">
                        <img class="footer-top__item-img" src="../assets/img/buy-comics-shop-locator.png">
                        <p>COMINCS SHOP LOCATOR</p>
                    </a>
                    <a href="#" class="footer-top__item">
                        <img class="footer-top__item-img" src="../assets/img/buy-dc-power-visa.svg">
                        <p>DC POWER PISA</p>
                    </a>
                </div>
            </div>
        </div>
        <div class="footer-mid">
            <div class="container">
                <div class="footer-mid__row">
                    <div class="footer-mid__col">
                        <h4>DC COMICS</h4>
                        <ul>
                            <li>Characters</li>
                            <li>Comics</li>
                            <li>Movies</li>
                            <li>TV</li>
                            <li>Games</li>
                            <li>Videos</li>
                            <li>News</li>
                        </ul>
                        <h4>Shop</h4>
                        <ul>
                            <li>Shop DC</li>
                            <li>Shop DC Collectibles</li>
                        </ul>
                    </div>
                    <div class="footer-mid__col">
                        <h4>DS</h4>
                        <ul>
                            <li>Terms Of Use</li>
                            <li>Privacy policy</li>
                            <li>Ad Choices</li>
                            <li>Advertising</li>
                            <li>Jobs</li>
                            <li>Subscriptions</li>
                            <li>Talent Workshops</li>
                            <li>CPSC Certificates</li>
                            <li>Ratings</li>
                            <li>Shop Help</li>
                            <li>Contact Us</li>
                        </ul>
                    </div>
                    <div class="footer-mid__col">
                        <h4>SITES</h4>
                        <ul>
                            <li>DC</li>
                            <li>MAD Magazine</li>
                            <li>DC Kids</li>
                            <li>DC Universe</li>
                            <li>DC Power Visa</li>
                        </ul>
                    </div>
                </div>
            </div>
        </div>
        <div class="footer-bottom">
            <div class="container">
                <div class="footer-bottom__wrapper">
                    <button>SING-UP NOW!</button>
                    <div class="footer-bottom__social">
                        <span>FOLLOW US</span>
                        <img src="../assets/img/footer-facebook.png">
                        <img src="../assets/img/footer-twitter.png">
                        <img src="../assets/img/footer-youtube.png">
                        <img src="../assets/img/footer-pinterest.png">
                        <img src="../assets/img/footer-periscope.png">
                    </div>
                </div>
            </div>
        </div>
    </footer>
</template>

<script>
export default {
    name: 'BaseFooter',
}
</script>

<style lang="scss" scoped>
.footer-top {
    background-color: var(--primary-color);
    padding: 1.875rem;
    &__items {
        display: flex;
        align-items: center;
        justify-content: space-around;
    }

    &__item {
        display: flex;
        align-items: center;
        color: #fff;
        text-decoration: none;
        &-img {
            height: 2.1875rem;
            margin-right: 0.625rem;
        }
    }
}
.footer-mid {
    background-image: url(../assets/img/footer-bg.jpg);
    background-repeat: no-repeat;
    background-size: cover;
    color: #797979;

    &__row {
        display: flex;
        background-image: url('../assets/img/dc-logo-bg.png');
        background-position: center right;
        background-repeat: no-repeat;
    }

    &__col {
        width: 8%;
        padding: 25px 0;
        margin: 0 8px;
        
        
        h4 {
            margin-bottom: .625rem;
            margin-top: .9375rem;
            color: #fff;
        }

        ul li {
            list-style-type: none;
            font-size: 0.75rem;
        }
    }
}
.footer-bottom {
    background-color: #303030;
    padding: 2.5rem 0;

    &__wrapper {
        display: flex;
        align-items: center;
        justify-content: space-between;

        & button {
            padding: .625rem;
            border: .125rem solid var(--primary-color);
            background-color: transparent;
            color: #fff;
        }
    }

    &__social {
        display: flex;
        align-items: center;

        & span {
            font-weight: 500;
            color: var(--primary-color);
            margin-right: 1.25rem;
        }

        & img {
            margin-right: 0.9375rem;
        }
    }
}
</style>