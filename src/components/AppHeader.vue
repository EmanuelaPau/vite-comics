<template>
    <header class="container">
        <img class="brand-logo" src="../assets/dc-logo.png" alt="dc comics brand logo in blue">
        <nav>
            <ul class="">
                <li class="" v-for="(element, index) in menuList"
                    @click="menuList[index].active == false ? menuList[index].active = true : menuList[index].active = false">
                    <a href="#" :class="menuList[index].active == true ? 'active' : ''">
                        {{ element.name }} <span class="underline"
                            :class="menuList[index].active == true ? '' : 'display-none'"></span>
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
                    active: false,
                },
                {
                    name: 'comics',
                    active: false,
                },
                {
                    name: 'movies',
                    active: false,
                },
                {
                    name: 'tv',
                    active: false,
                },
                {
                    name: 'games',
                    active: false,
                },
                {
                    name: 'collectibles',
                    active: false,
                },
                {
                    name: 'videos',
                    active: false,
                },
                {
                    name: 'fans',
                    active: false,
                },
                {
                    name: 'news',
                    active: false,
                },
                {
                    name: 'shop',
                    active: false,
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

    .underline {
        position: absolute;
        top: calc(100% + 1rem - 5px);
        left: 0;
        transform: translateX(-.5rem);

        width: calc(100% - 1rem);
        margin: 0 1rem;
        height: 5px;
        background-color: $primaryColor;
    }

    nav {
        height: 80px;
        // height: calc(100% + 2rem);

        ul {
            @include flex(row, center, center);
            height: 100%;

            li {
                position: relative;
                text-transform: uppercase;
                height: 100%;

                display: flex;
                align-items: center;

                a {
                    text-decoration: none;
                    color: $secondaryColor;
                    font-size: .9rem;
                    font-weight: 600;
                    margin: 1rem;
                }

                a:hover {
                    color: $tertiaryColor ;
                }
            }
        }
    }
}
</style>
