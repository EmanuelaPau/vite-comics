<template>
    <footer>
        <div class="footer-nav">

            <div class="nav-menu container">

                <div class="nav-column">
                    <div class="nav-col-ul-container">
                        <div class="ul-list-container">
                            <h3>Dc comics</h3>
                            <ul>
                                <li>
                                    <a href="">
                                        Characters
                                    </a>
                                </li>

                                <li>
                                    <a href="">
                                        Characters
                                    </a>
                                </li>

                                <li>
                                    <a href="">
                                        Characters
                                    </a>
                                </li>

                                <li>
                                    <a href="">
                                        Characters
                                    </a>
                                </li>

                                <li>
                                    <a href="">
                                        Characters
                                    </a>
                                </li>

                                <li>
                                    <a href="">
                                        Characters
                                    </a>
                                </li>

                                <li>
                                    <a href="">
                                        Characters
                                    </a>
                                </li>
                            </ul>
                        </div>
                        <div class="ul-list-container">
                            <h3>Shop</h3>
                            <ul>
                                <li>
                                    <a href="">
                                        Characters
                                    </a>
                                </li>

                                <li>
                                    <a href="">
                                        Characters
                                    </a>
                                </li>
                            </ul>
                        </div>
                    </div>


                </div>

                <div class="nav-column">
                    <div class="nav-col-ul-container">
                        <div class="ul-list-container">
                            <h3>Dc</h3>
                            <ul>
                                <li>
                                    <a href="">
                                        Characters
                                    </a>
                                </li>

                                <li>
                                    <a href="">
                                        Characters
                                    </a>
                                </li>

                                <li>
                                    <a href="">
                                        Characters
                                    </a>
                                </li>

                                <li>
                                    <a href="">
                                        Characters
                                    </a>
                                </li>

                                <li>
                                    <a href="">
                                        Characters
                                    </a>
                                </li>

                                <li>
                                    <a href="">
                                        Characters
                                    </a>
                                </li>

                                <li>
                                    <a href="">
                                        Characters
                                    </a>
                                </li>

                                <li>
                                    <a href="">
                                        Characters
                                    </a>
                                </li>

                                <li>
                                    <a href="">
                                        Characters
                                    </a>
                                </li>

                                <li>
                                    <a href="">
                                        Characters
                                    </a>
                                </li>

                                <li>
                                    <a href="">
                                        Characters
                                    </a>
                                </li>
                            </ul>
                        </div>
                    </div>

                    <div class="nav-col-ul-container">
                        <h1></h1>
                        <ul>
                            <li></li>
                        </ul>
                    </div>
                </div>

                <div class="nav-column">
                    <div class="nav-col-ul-container">
                        <div class="ul-list-container">
                            <h3>Sites</h3>
                            <ul>
                                <li>
                                    <a href="">
                                        Characters
                                    </a>
                                </li>

                                <li>
                                    <a href="">
                                        Characters
                                    </a>
                                </li>

                                <li>
                                    <a href="">
                                        Characters
                                    </a>
                                </li>

                                <li>
                                    <a href="">
                                        Characters
                                    </a>
                                </li>

                                <li>
                                    <a href="">
                                        Characters
                                    </a>
                                </li>
                            </ul>
                        </div>
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

                <a href="">
                    <img src="../assets/footer-facebook.png" alt="#">
                </a>

                <a href="">
                    <img src="../assets/footer-facebook.png" alt="#">
                </a>

                <a href="">
                    <img src="../assets/footer-facebook.png" alt="#">
                </a>

                <a href="">
                    <img src="../assets/footer-facebook.png" alt="#">
                </a>

                <a href="">
                    <img src="../assets/footer-facebook.png" alt="#">
                </a>
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
        color: $colorLight;
        width: 100%;
        height: 400px;
        background-image: url('../assets/footer-bg.jpg');
        background-repeat: none;
        background-size: cover;
        padding: 2rem;

        .nav-menu {
            @include flex(row, left, start);

            .nav-column {

                .nav-col-ul-container {
                    .ul-list-container {
                        margin-bottom: 1.3rem;
                        margin-right: 2.5rem;

                        h3 {
                            margin-bottom: 1rem;
                            text-transform: uppercase;
                        }

                        ul {
                            li {
                                margin-bottom: .5rem;

                                a {
                                    color: $tertiaryColor;
                                }
                            }
                        }
                    }
                }
            }

        }

    }

    .footer-cta {
        @include flex(row, space-between, center);
        padding: 2rem;

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

