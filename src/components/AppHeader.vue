<template>
    <header class="">
        <img class="brand-logo" src="" alt="dc comics brand logo in blue">
        <nav>
            <ul class="">
                <li>
                    characters
                </li>
                <li>
                    comics
                </li>
                <li>
                    movies
                </li>
                <li>
                    tv
                </li>
                <li>
                    games
                </li>
                <li>
                    collectibles
                </li>
                <li>
                    videos
                </li>
                <li>
                    fans
                </li>
                <li>
                    news
                </li>
                <li>
                    shop
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
    padding: 2rem;

}
</style>
