<script>
export default {
    name: 'AppMain',
    props: ['infoMain'],
    methods: {
        createImagePath(img) {
            const url = new URL(`../assets/img/${img}`, import.meta.url);
            return url.href
        }
    },
}
</script>

<template>
    <section id="films">
    </section>
    <section id="infoMain">
        <ul>
            <li v-for="info in infoMain">
                <a href="#">
                    <img :src="createImagePath(info.url)" alt="">
                    <p>{{ info.text }}</p>
                </a>
            </li>
        </ul>
    </section>
</template>

<style lang="scss" scoped>
#films {
    background-color: #1c1c1c;
}

#infoMain {
    background-color: #0282f9;
    padding: 30px 0;

    ul {
        display: flex;
        justify-content: center;
        align-items: center;
        gap: 40px;

        li {

            a {
                display: flex;
                align-items: center;

                img {
                    display: block;
                    width: 40px;
                    height: 40px;
                    margin-right: 5px;
                }

                p {
                    color: white;
                    text-transform: uppercase;
                    font-size: 0.8rem;
                }
            }
        }
    }
}
</style>