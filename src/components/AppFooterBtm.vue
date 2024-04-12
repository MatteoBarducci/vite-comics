<script>
    export default{
        name: 'AppFooterBtm',
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
    <section>
        <div class="main-container">
            <div class="footer-btm-left">
                <button><h3>SIGN UP NOW!</h3></button>
            </div>
    
            <div class="footer-btm-right">
                <h2>FOLLOW US</h2>
                <ul>
                    <li><a href="#"><img src="../assets/img/footer-facebook.png"></a></li>
                    <li><a href="#"><img src="../assets/img/footer-periscope.png"></a></li>
                    <li><a href="#"><img src="../assets/img/footer-pinterest.png"></a></li>
                    <li><a href="#"><img src="../assets/img/footer-youtube.png"></a></li>
                    <li><a href="#"><img src="../assets/img/footer-twitter.png"></a></li>
                </ul>
            </div>
        </div>
    </section>
</template>

<style scoped lang="scss">
@use '../style/partials/variables.scss' as *;

    section{
        background-color: #303030;
    }

    .main-container{
        padding: 26px;
        display: flex;
        justify-content: space-between;
        align-items: center;

        button{
            padding: 14px;
            background-color: #303030;
            border: 2px solid $brand-primary;
            color: white;
        }

        .footer-btm-right{
            display: flex;
            align-items: center;
            gap: 30px;

            h2{
                color: $brand-primary;
            }

            ul{
                display: flex;
                gap: 20px;
            }
        }
    }

</style>