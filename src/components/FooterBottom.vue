<script>
import _socials from '../assets/data/_socials';

export default {
    name: 'FooterBottom',
    props: ['socials'],
    methods: {
        createImagePath(img) {
            const url = new URL(`../assets/img/${img}`, import.meta.url);
            return url.href
        }
    },
}
</script>

<template>
    <footer class="footer-bottom">
        <div class="container">
            <div>
                <a class="btn" href="#">SIGN-UP NOW!</a>
            </div>
            <div>
                <h4>FOLLOW US</h4>
                <ul>
                    <li v-for="social in socials">
                        <a href="#">
                            <img :src="createImagePath(social.url)" :alt="social.text">
                        </a>
                    </li>
                </ul>
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