<template>
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
                    <img class="card-img" src="../assets/buy-comics-merchandise.png"
                        alt="sylized dc comics logo inside an ipad">
                    <h3>
                        Dc Merchandise
                    </h3>
                </a>
            </div>

            <div class="card">
                <a href="">
                    <img class="card-img" src="../assets/buy-comics-subscriptions.png"
                        alt="sylized dc comics logo inside an ipad">
                    <h3>
                        Subscription
                    </h3>
                </a>
            </div>

            <div class="card">
                <a href="">
                    <img class="card-img" src="../assets/buy-comics-shop-locator.png"
                        alt="sylized dc comics logo inside an ipad">
                    <h3>
                        Comic Shop Locator
                    </h3>
                </a>
            </div>

            <div class="card">
                <a href="">
                    <img class="card-img" src="../assets/buy-dc-power-visa.svg" alt="sylized dc comics logo inside an ipad">
                    <h3>
                        Dc Power Visa
                    </h3>
                </a>
            </div>

        </div>
    </div>
</template>

<script>

export default {
    name: 'AppMainSelection',
    data() {
        return {
        }
    },
    methods() {
    },
}		
</script>
<style scoped lang="scss">
@import '../styles/partials/_variables.scss';
@import '../styles/partials/_mixins.scss';

div.selection {
    color: $colorLight;
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
                    height: 45px;
                    margin-right: 1.3rem;
                }

                h3 {
                    font-size: .8rem;
                    font-weight: 500;
                }
            }
        }
    }
}
</style>

