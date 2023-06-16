<template>
    <div class="comics-card">
        <div class="img-container">
            <img :src="comicsTumbnail" alt="">
            <p>{{ comicsName }}</p>
        </div>
    </div>
</template>

<script>

export default {
    name: 'AppMainSelection',

    props: {
        comicsTumbnail: String,
        comicsName: String,
    },

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

div.comics-card {

    div.img-container {
        width: 140px;
        height: 150px;
        margin-bottom: 5rem;

        img {
            width: 100%;
            height: 100%;
            object-fit: cover;
            object-position: top;
            margin-bottom: .7rem;
        }

        p {
            text-transform: uppercase;
            font-size: .75rem;
        }
    }

}
</style>

