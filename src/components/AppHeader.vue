<template>
    <header class="container">
        <img class="brand-logo" src="../assets/dc-logo.png" alt="dc comics brand logo in blue">
        <nav>
            <ul class="">
                <li>
                    <a href="#">
                        characters
                    </a>
                </li>
                <li>
                    <a href="#">
                        comics
                    </a>

                </li>
                <li>
                    <a href="#">
                        movies
                    </a>
                </li>
                <li>
                    <a href="#">
                        tv
                    </a>
                </li>
                <li>
                    <a href="#">
                        games
                    </a>
                </li>
                <li>
                    <a href="#">
                        collectables
                    </a>
                </li>
                <li>
                    <a href="#">
                        videos
                    </a>
                </li>
                <li>
                    <a href="#">
                        fans
                    </a>
                </li>
                <li>
                    <a href="#">
                        news
                    </a>
                </li>
                <li>
                    <a href="#">
                        shop
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
            }
        }
    }
}
</style>
