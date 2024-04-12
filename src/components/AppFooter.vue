<script>
    export default{
        name: 'AppFooter',
        data() {
            return{
                links: {}
            }
        },
        methods: {
            getImageUrl(name) {
                return new URL(`${name}`, import.meta.url).href
            }
        }
    }
</script>

<template>
    <footer>
        <div class="main-container">
            <div class="footer-left">
                <div>
                    <div>
                        <h2>DC COMICS</h2>
                        <ul>
                            <li><a href="#">Characters</a></li>
                            <li><a href="#">Comics</a></li>
                            <li><a href="#">Movies</a></li>
                            <li><a href="#">TV</a></li>
                            <li><a href="#">Games</a></li>
                            <li><a href="#">Videos</a></li>
                            <li><a href="#">News</a></li>
                        </ul>
                    </div>
                    <div id="margin-top">
                        <h2>SHOP</h2>
                        <ul>
                            <li><a href="#">Shop DC</a></li>
                            <li><a href="#">Shop DC Collectibles</a></li>
                        </ul>
                    </div>
                </div>

                <div>
                    <h2>DC</h2>
                    <ul>
                        <li><a href="#">Term Of Use</a></li>
                        <li><a href="#">Privacy policy (New)</a></li>
                        <li><a href="#">Ad Choices</a></li>
                        <li><a href="#">Jobs</a></li>
                        <li><a href="#">Subscriptions</a></li>
                        <li><a href="#">Talent Workshops</a></li>
                        <li><a href="#">CPSC certificates</a></li>
                        <li><a href="#">Ratings</a></li>
                        <li><a href="#">Shop Help</a></li>
                        <li><a href="#">Contact Us</a></li>
                        <li><a href="#">Advertising</a></li>
                    </ul>
                </div>
                <div>
                    <h2>SITES</h2>
                    <ul>
                        <li><a href="#">DC</a></li>
                        <li><a href="#">MAD Magazine</a></li>
                        <li><a href="#">DC Kids</a></li>
                        <li><a href="#">DC Universe</a></li>
                        <li><a href="#">DC Power Visa</a></li>
                    </ul>
                </div>
            </div>
            <div class="footer-right"></div>
        </div>
    </footer>
</template>

<style scoped lang="scss">
@use '../style/partials/variables.scss' as *;

    footer{
        background-image: url('src/assets/img/footer-bg.jpg');
    }

    .main-container{
        display: flex;
        justify-content: space-between;
        height: 390px;
    }
    .footer-left{
        padding: 40px;
        width: 30%;
        display: flex;
        color: white;
        gap: 40px;
        white-space:nowrap;

        h2{
            margin-bottom: 10px;
        }

        li{
            margin-bottom: 5px;

            a{
                color: #959595;
            }
        }  
    }

    #margin-top{
        margin-top: 10px;
    }
    .footer-right {
        background-image: url('../assets/img/dc-logo-bg.png');
        background-size: cover;
        background-position: center;
        background-repeat: no-repeat;
        width: 40%;
        height: 100%;
    }

</style>