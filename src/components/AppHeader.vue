<template>
    <header class="container">
        <img class="brand-logo" src="../assets/dc-logo.png" alt="dc comics brand logo in blue">
        <nav>
            <ul class="">
                <li>
                    <a href="#" class="" v-for="element in menuList">
                        {{ element.name }}
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
                    name: 'characters',
                    active: true,
                },
                {
                    name: 'comics',
                    active: true,
                },
                {
                    name: 'movies',
                    active: true,
                },
                {
                    name: 'tv',
                    active: true,
                },
                {
                    name: 'games',
                    active: true,
                },
                {
                    name: 'collectibles',
                    active: true,
                },
                {
                    name: 'videos',
                    active: true,
                },
                {
                    name: 'fans',
                    active: true,
                },
                {
                    name: 'news',
                    active: true,
                },
                {
                    name: 'shop',
                    active: true,
                },
            ],
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

    .active {
        color: $primaryColor;
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
