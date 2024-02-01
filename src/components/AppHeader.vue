<script>
export default {
    name: 'AppHeader',
    data: () => ({
        links: [
            {
                text: 'Characters',
                url: '#',
                current: false,
            },
            {
                text: 'Comics',
                url: '#',
                current: true,
            },
            {
                text: 'Movies',
                url: '#',
                current: false,
            },
            {
                text: 'TV',
                url: '#',
                current: false,
            },
            {
                text: 'Games',
                url: '#',
                current: false,
            },
            {
                text: 'Collectibles',
                url: '#',
                current: false,
            },
            {
                text: 'Videos',
                url: '#',
                current: false,
            },
            {
                text: 'Fans',
                url: '#',
                current: false,
            },
            {
                text: 'News',
                url: '#',
                current: false,
            },
            {
                text: 'Shop',
                url: '#',
                current: false,
            },
        ]
    })
}
</script>

<template>
    <header class="border">
        <nav class="container">
            <figure>
                <img src="../assets/img/dc-logo.png" alt="">
            </figure>
            <ul>
                <li v-for="link in links"><a href="#">{{ link.text }}</a></li>
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