<script>
export default {
    name: 'AppFooter',
}
</script>

<template>
    <footer>
        <div class="footer-top">
            <div class="container">
                <p>lista e immagine</p>
            </div>
        </div>
        <div class="footer-bottom">
            <div class="container">
                <p>registrazione e social</p>
            </div>
        </div>
    </footer>
</template>

<style scoped>
.footer-top {
    height: 250px;
    background-image: url(../assets/img/footer-bg.jpg);
    background-size: cover;
    background-repeat: no-repeat;
}


.footer-bottom {
    height: 65px;
    background-color: #303030;
}
</style>