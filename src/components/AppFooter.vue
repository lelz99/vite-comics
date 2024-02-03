<script>
import FooterTop from './FooterTop.vue';
export default {
    name: 'AppFooter',
    components: { FooterTop, }
}
</script>

<template>
    <FooterTop />
    <footer>
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