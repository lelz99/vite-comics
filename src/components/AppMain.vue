<script>
export default {
    name: 'AppMain',
    props: ['infoMain', 'films'],
    methods: {
        createImagePath(img) {
            const url = new URL(`../assets/img/${img}`, import.meta.url);
            return url.href
        }
    },
}
</script>

<template>
    <section id="jumbotron">
        <figure></figure>
    </section>
    <section id="films">
        <div class="container">
            <div class="label">CURRENT SERIES</div>
            <div class="row">
                <div v-for="film in films" class="col">
                    <div class="card">
                        <img :src="film.thumb" alt="">
                        <h4>{{ film.series }}</h4>
                    </div>
                </div>
            </div>
        </div>
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
#jumbotron {

    figure {
        background-image: url(../assets/img/jumbotron.jpg);
        background-size: cover;
        background-repeat: no-repeat;
        height: 400px;
        display: block;
    }
}

#films {
    background-color: #1c1c1c;
    padding: 20px;

    .label {
        width: 180px;
        height: 40px;
        background-color: #0282f9;
        color: white;
        font-weight: bold;
        text-align: center;
        padding: 10px 0;

        position: relative;
        bottom: 40px;
        left: 0;
    }

    .row {
        display: flex;
        flex-wrap: wrap;
        justify-content: center;
        margin: 0 -10px;
    }

    .col {
        flex-basis: calc(100% / 6);
        padding: 10px;

        .card {

            img {
                display: block;
                max-width: 100%;
            }

            h4 {
                color: white;
                text-align: center;
                margin-top: 5px;
            }
        }
    }
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