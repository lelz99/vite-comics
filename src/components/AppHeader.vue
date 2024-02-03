<script>
export default {
    name: 'AppHeader',
    data: () => ({}),
    props: ['headerLinks']
}
</script>

<template>
    <header class="border">
        <nav class="container">
            <figure>
                <img src="../assets/img/dc-logo.png" alt="">
            </figure>
            <ul>
                <li v-for="link in headerLinks"><a href="#">{{ link.text }}</a></li>
            </ul>
        </nav>
    </header>
</template>

<style scoped>
header {
    background-color: white;
    padding: 20px 0;
}

nav {
    display: flex;
    justify-content: space-between;
    align-items: center;
}

ul {
    display: flex;
    gap: 20px;
    font-weight: bold;
    font-size: 0.8rem;
    text-transform: uppercase;
}

img {
    display: block;
    width: 70px;
}
</style>