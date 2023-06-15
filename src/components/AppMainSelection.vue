<template>
    <main>
        <div class="content">
            <div class="container">
                <h2>Content goes here</h2>
            </div>
        </div>
        <div class="selection">
            <div class="container">

                <div class="card">
                    <a href="">
                        <img class="card-img" src="../assets/buy-comics-digital-comics.png"
                            alt="sylized dc comics logo inside an ipad">
                        <h3>
                            Digital Comics
                        </h3>
                    </a>
                </div>

                <div class="card">
                    <a href="">
                        <img class="card-img" src="../assets/buy-comics-digital-comics.png"
                            alt="sylized dc comics logo inside an ipad">
                        <h3>
                            Digital Comics
                        </h3>
                    </a>
                </div>

                <div class="card">
                    <a href="">
                        <img class="card-img" src="../assets/buy-comics-digital-comics.png"
                            alt="sylized dc comics logo inside an ipad">
                        <h3>
                            Digital Comics
                        </h3>
                    </a>
                </div>

                <div class="card">
                    <a href="">
                        <img class="card-img" src="../assets/buy-comics-digital-comics.png"
                            alt="sylized dc comics logo inside an ipad">
                        <h3>
                            Digital Comics
                        </h3>
                    </a>
                </div>

                <div class="card">
                    <a href="">
                        <img class="card-img" src="../assets/buy-comics-digital-comics.png"
                            alt="sylized dc comics logo inside an ipad">
                        <h3>
                            Digital Comics
                        </h3>
                    </a>
                </div>

            </div>
        </div>

    </main>
</template>

<script>

export default {
    name: 'AppMainSelection',
    data() {
        return {
            links: [
                'gino',
                'ciao',
            ]
        }
    },
    methods() {
    },
}		
</script>
<style scoped lang="scss">
@import '../styles/partials/_variables.scss';
@import '../styles/partials/_mixins.scss';

main {
    color: $colorLight;

    div.content {
        background-color: $quaternaryColor;
        width: 100%;
        padding: 3rem;
    }

    div.selection {
        background-color: $primaryColor;
        width: 100%;
        padding: 3rem;
        text-transform: uppercase;

        div.container {
            @include flex(row, space-between, center);

            div.card {
                margin: 0 2rem;

                a {
                    color: $colorLight;
                    text-decoration: none;
                    @include flex(row, center, center);

                    img {
                        height: 50px;
                        margin-right: 1.3rem;
                    }

                    h3 {
                        font-size: 1rem;
                    }
                }
            }
        }
    }
}
</style>

