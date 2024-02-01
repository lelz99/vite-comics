<script>
export default {
    name: 'AppFooter',
}
</script>

<template>
    <footer>
        <div class="footer-top">
            <div class="container">
                <div class="row">
                    <div class="col-40">
                        <div class="card">
                            <h3>DC COMICS</h3>
                            <ul>
                                <li><a href="#">Characters</a></li>
                                <li><a href="#">Comics</a></li>
                                <li><a href="#">Movies</a></li>
                                <li><a href="#">TV</a></li>
                                <li><a href="#">Games</a></li>
                                <li><a href="#">Videos</a></li>
                                <li><a href="#">News</a></li>
                            </ul>
                            <h3>SHOP</h3>
                            <ul>
                                <li><a href="#">Shop DC</a></li>
                                <li><a href="#">Shop DC Collectibles</a></li>
                            </ul>
                        </div>
                        <div class="card">
                            <h3>DC</h3>
                            <ul>
                                <li><a href="#">Terms Of Use</a></li>
                                <li><a href="#">Privacy policy</a></li>
                                <li><a href="#">Ad Choices</a></li>
                                <li><a href="#">Advertising</a></li>
                                <li><a href="#">Jobs</a></li>
                                <li><a href="#">Subscriptions</a></li>
                                <li><a href="#">Talent Workshops</a></li>
                                <li><a href="#">CPSC Certificates</a></li>
                                <li><a href="#">Ratings</a></li>
                                <li><a href="#">Shop Help</a></li>
                                <li><a href="#">Contacts Us</a></li>
                            </ul>
                        </div>
                        <div class="card">
                            <h3>SITES</h3>
                            <ul>
                                <li><a href="#">DC</a></li>
                                <li><a href="#">MAD Magazine</a></li>
                                <li><a href="#">DC Kids</a></li>
                                <li><a href="#">DC Universe</a></li>
                                <li><a href="#">DC Power Visa</a></li>
                            </ul>
                        </div>
                        <div class="card">

                        </div>
                    </div>
                    <div class="col-60">
                        <figure>
                            <img src="../assets/img/dc-logo-bg.png" alt="">
                        </figure>
                    </div>
                </div>
            </div>
        </div>
        <div class="footer-bottom">
            <div class="container">
                <div>
                    <a class="btn" href="#">SIGN-UP NOW!</a>
                </div>
                <div>
                    <h4>FOLLOW US</h4>
                    <ul>
                        <li><a href="#"><img src="../assets/img/footer-facebook.png" alt=""></a></li>
                        <li><a href="#"><img src="../assets/img/footer-twitter.png" alt=""></a></li>
                        <li><a href="#"><img src="../assets/img/footer-youtube.png" alt=""></a></li>
                        <li><a href="#"><img src="../assets/img/footer-pinterest.png" alt=""></a></li>
                        <li><a href="#"><img src="../assets/img/footer-periscope.png" alt=""></a></li>
                    </ul>
                </div>
            </div>
        </div>
    </footer>
</template>

<style>
.footer-top {
    background-image: url(../assets/img/footer-bg.jpg);
    background-size: cover;
    background-repeat: no-repeat;

    .row {
        display: flex;
        padding: 20px 0;

        .col-40 {
            flex-basis: 40%;
            display: flex;
            flex-wrap: wrap;

            .card {
                flex-basis: calc(100% / 3);

                h3 {
                    color: white;
                    margin: 10px 0;
                }

                a {
                    color: gray;
                    font-size: 0.7rem;
                }
            }

        }

        .col-60 {
            flex-basis: 60%;

            img {
                width: 200px
            }
        }
    }

}


.footer-bottom {
    background-color: #303030;

    div {
        padding: 10px 0;

        .btn {
            color: white;
            border: 2px solid #0282f9;
            padding: 10px;
        }
    }

    div {
        display: flex;
        justify-content: space-between;
        font-weight: bold;

        div {
            display: flex;
            gap: 20px;
            align-items: center;

            h4 {
                color: #0282f9;
            }

            ul {
                display: flex;
                gap: 15px;
            }
        }
    }
}
</style>