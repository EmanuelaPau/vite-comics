<template>
    <main>
        <div class="content">
            <div class="container">
                <h2>Content goes here</h2>
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

}
</style>

