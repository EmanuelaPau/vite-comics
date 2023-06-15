<template>
    <footer>
        <div class="footer-nav">

            <div class="container">
                <div class="nav-menu">

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
                                            Comics
                                        </a>
                                    </li>

                                    <li>
                                        <a href="">
                                            Movies
                                        </a>
                                    </li>

                                    <li>
                                        <a href="">
                                            TV
                                        </a>
                                    </li>

                                    <li>
                                        <a href="">
                                            Games
                                        </a>
                                    </li>

                                    <li>
                                        <a href="">
                                            Videos
                                        </a>
                                    </li>

                                    <li>
                                        <a href="">
                                            News
                                        </a>
                                    </li>
                                </ul>
                            </div>
                            <div class="ul-list-container">
                                <h3>Shop</h3>
                                <ul>
                                    <li>
                                        <a href="">
                                            Shop Dc
                                        </a>
                                    </li>

                                    <li>
                                        <a href="">
                                            Shop Dc Collectibles
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
                                            Terms of use
                                        </a>
                                    </li>

                                    <li>
                                        <a href="">
                                            Privacy policy (New)
                                        </a>
                                    </li>

                                    <li>
                                        <a href="">
                                            Ad Choices
                                        </a>
                                    </li>

                                    <li>
                                        <a href="">
                                            Advertising
                                        </a>
                                    </li>

                                    <li>
                                        <a href="">
                                            Jobs
                                        </a>
                                    </li>

                                    <li>
                                        <a href="">
                                            Subscriptions
                                        </a>
                                    </li>

                                    <li>
                                        <a href="">
                                            Talent Workshops
                                        </a>
                                    </li>

                                    <li>
                                        <a href="">
                                            CPSC Certificates
                                        </a>
                                    </li>

                                    <li>
                                        <a href="">
                                            Ratings
                                        </a>
                                    </li>

                                    <li>
                                        <a href="">
                                            Shop Help
                                        </a>
                                    </li>

                                    <li>
                                        <a href="">
                                            Contact Us
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
                                            DC
                                        </a>
                                    </li>

                                    <li>
                                        <a href="">
                                            MAD Magazine
                                        </a>
                                    </li>

                                    <li>
                                        <a href="">
                                            DC Kids
                                        </a>
                                    </li>

                                    <li>
                                        <a href="">
                                            DC Universe
                                        </a>
                                    </li>

                                    <li>
                                        <a href="">
                                            DC Power Visa
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

                <img src="../assets/dc-logo-bg.png" alt="">
            </div>

        </div>
        <div class="footer-cta container">
            <button class="button-cta">Sign-up now!</button>

            <nav>
                <a class="cta-txt" href="">
                    follow us
                </a>

                <a href="">
                    <img src="../assets/footer-facebook.png" alt="#">
                </a>

                <a href="">
                    <img src="../assets/footer-twitter.png" alt="#">
                </a>

                <a href="">
                    <img src="../assets/footer-youtube.png" alt="#">
                </a>

                <a href="">
                    <img src="../assets/footer-pinterest.png" alt="#">
                </a>

                <a href="">
                    <img src="../assets/footer-periscope.png" alt="#">
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
        background-image: url('../assets/footer-bg.jpg');
        background-repeat: none;
        background-size: cover;
        overflow: hidden;

        div.container {
            @include flex(row, space-between, center);
            height: 450px;

            .nav-menu {
                @include flex(row, left, start);
                width: 50%;
                padding: 2rem;

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
                                        font-size: .9rem;
                                    }
                                }
                            }
                        }
                    }
                }

            }

            img {
                // height: 100%;
                width: 40%;

            }
        }
    }

    button.button-cta {
        border-radius: none;
        border: 1px solid $primaryColor;
        background-color: $secondaryColor;
        color: $colorLight;
        text-transform: uppercase;
        font-size: .9rem;
        padding: .7rem 1rem;
    }

    .footer-cta {
        @include flex(row, space-between, center);
        padding: 2rem;


        nav {
            @include flex(row, space-between, center);

            a.cta-txt {
                color: $primaryColor;
                text-transform: uppercase;
                margin-right: 12px;
                font-size: 1.2rem;
                font-weight: 600;
            }

            img {
                margin: 7px;
                width: 30px;
            }
        }
    }
}
</style>

