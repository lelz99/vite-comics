<script>
export default {
    name: 'FooterTop',
    props: ['otherSitesLinks', 'listLinks', 'infoLinks']
}
</script>

<template>
    <footer class="footer-top">
        <div class="container">
            <div class="row">
                <div class="col-40">
                    <div class="card">
                        <h3>DC COMICS</h3>
                        <ul>
                            <li v-for="link in listLinks"><a href="#">{{ link.text }}</a></li>
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
                            <li v-for="info in infoLinks"><a href="#">{{ info.text }}</a></li>
                        </ul>
                    </div>
                    <div class="card">
                        <h3>SITES</h3>
                        <ul>
                            <li v-for="site in otherSitesLinks"><a href="#">{{ site.text }}</a></li>
                        </ul>
                    </div>
                </div>
                <div class="col-60">
                    <figure>
                        <img src="../assets/img/dc-logo-bg.png" alt="">
                    </figure>
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
                    margin: 5px 0;
                }

                a {
                    color: gray;
                    font-size: 0.7rem;
                }
            }

        }

        .col-60 {
            flex-basis: 60%;
            text-align: end;

            img {
                width: 50%;
                height: 50%;
            }
        }
    }

}
</style>