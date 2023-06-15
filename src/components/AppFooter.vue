<template>
    <footer>
        <div class="footer-nav">

            <div class="nav-menu">
                <div class="nav-column">
                    <div class="nav-col-ul-container">
                        <h1></h1>
                        <ul>
                            <li></li>
                        </ul>
                    </div>

                    <div class="nav-col-ul-container">
                        <h1></h1>
                        <ul>
                            <li></li>
                        </ul>
                    </div>
                </div>
            </div>
            <div class="nav-img">
                <img src="" alt="">
            </div>

        </div>

        <div class="footer-cta container">
            <button>Sign-up-now!</button>

            <nav>
                <a href="">
                    follow us
                </a>

                <img src="../assets/footer-facebook.png" alt="#">
                <img src="../assets/footer-facebook.png" alt="#">
                <img src="../assets/footer-facebook.png" alt="#">
                <img src="../assets/footer-facebook.png" alt="#">
                <img src="../assets/footer-facebook.png" alt="#">

            </nav>

        </div>
    </footer>
</template>

<script>

export default {
    name: 'AppFooter',
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

footer {
    background-color: $secondaryColor;
    height: 600px;

    .footer-nav {
        width: 100%;
        height: 400px;
        background-image: url('../assets/footer-bg.jpg');
        background-repeat: none;
        background-size: cover;
    }

    .footer-cta {
        @include flex(row, space-between, center);
        padding: 1.3rem;

        nav {
            @include flex(row, space-between, center);

            a {
                color: $primaryColor;
                text-transform: uppercase;
                margin-right: 12px;
            }

            img {
                margin: 7px;
                width: 30px;
            }
        }
    }
}
</style>

