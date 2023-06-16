<template>
    <footer>
        <div class="footer-nav">

            <div class="container">
                <div class="nav-menu">

                    <div v-for="(sections, index) in navLinks" class="ul-list-container">
                        <h3>{{ sections.title }}</h3>
                        <ul>
                            <li v-for="(links) in navLinks[index].pages">
                                <a href="">
                                    {{ links }}
                                </a>
                            </li>
                        </ul>
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
            navLinks: [
                {
                    title: 'DC Comics',
                    pages:
                        [
                            'Characters',
                            'Comics',
                            'Movies ',
                            'TV',
                            'Games',
                            'Videos',
                            'News'
                        ],
                },
                {
                    title: 'Shop',
                    pages:
                        [
                            'Shop DC',
                            'Shop DC Collectibles',
                        ],
                },
                {
                    title: 'DC',
                    pages:
                        [
                            'Terms of use',
                            'Privacy Policy (New)',
                            'Ad Choices',
                            'Advertising',
                            'Jobs',
                            'Subscriptions',
                            'Talent Workshops',
                            'CPSC Certificater',
                            'Ratings',
                            'Shop Help',
                            'Contact Us',
                        ],
                },

                {
                    title: 'Sites',
                    pages:
                        [
                            'DC',
                            'MAD Magazine',
                            'DC Kids',
                            'DC Universe',
                            'DC Power Visa',
                        ],
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
                @include flex(column, left, start);
                flex-wrap: wrap;
                height: 100%;
                width: 50%;
                padding: 2rem;

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

