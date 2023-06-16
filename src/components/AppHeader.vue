<template>
    <header class="container">
        <img class="brand-logo" src="../assets/dc-logo.png" alt="dc comics brand logo in blue">
        <nav>
            <ul class="">
                <li>
                    <a href="#">

                    </a>
                </li>
            </ul>
        </nav>
    </header>
</template>

<script>

export default {
    name: 'AppHeader',
    data() {
        return {
            menuList: [
                {
                    name: characters,
                    active: false,
                },

                {
                    name: comics,
                    active: false,
                },

                {
                    name: movies,
                    active: false,
                },

                {
                    name: tv,
                    active: false,
                },

                {
                    name: games,
                    active: false,
                },

                {
                    name: collectables,
                    active: false,
                },

                {
                    name: videos,
                    active: false,
                },

                {
                    name: fans,
                    active: false,
                },

                {
                    name: news,
                    active: false,
                },

                {
                    name: shop,
                    active: false,
                },

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

header {
    padding: 1rem;
    // background-color: aqua;
    @include flex(row, space-between, center);

    img.brand-logo {
        width: 80px
    }

    ul {
        @include flex(row, center, center);

        li {
            margin: 1rem;
            text-transform: uppercase;

            a {
                text-decoration: none;
                color: $secondaryColor;
                font-size: .9rem;
                font-weight: 600;
            }
        }
    }
}
</style>
