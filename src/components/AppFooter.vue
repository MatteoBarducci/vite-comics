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
                            <li><a href="#">text</a></li>
                            <li><a href="#">text</a></li>
                            <li><a href="#">text</a></li>
                            <li><a href="#">text</a></li>
                            <li><a href="#">text</a></li>
                            <li><a href="#">text</a></li>
                            <li><a href="#">text</a></li>
                        </ul>
                    </div>
                    <div>
                        <h2>SHOP</h2>
                        <ul>
                            <li><a href="#">text</a></li>
                            <li><a href="#">text</a></li>
                        </ul>
                    </div>
                </div>

                <div>
                    <h2>DC</h2>
                    <ul>
                        <li><a href="#">text</a></li>
                        <li><a href="#">text</a></li>
                        <li><a href="#">text</a></li>
                        <li><a href="#">text</a></li>
                        <li><a href="#">text</a></li>
                        <li><a href="#">text</a></li>
                        <li><a href="#">text</a></li>
                        <li><a href="#">text</a></li>
                        <li><a href="#">text</a></li>
                        <li><a href="#">text</a></li>
                        <li><a href="#">text</a></li>
                    </ul>
                </div>
                <div>
                    <h2>SITES</h2>
                    <ul>
                        <li><a href="#">text</a></li>
                        <li><a href="#">text</a></li>
                        <li><a href="#">text</a></li>
                        <li><a href="#">text</a></li>
                        <li><a href="#">text</a></li>
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
    .footer-right {
        background-image: url('../assets/img/dc-logo-bg.png');
        background-size: cover;
        background-position: center;
        background-repeat: no-repeat;
        width: 40%;
        height: 100%;
    }



    

</style>