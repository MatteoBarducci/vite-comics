<script>
    export default{
        name: 'AppLowerSection',
        data() {
            return{
                labels: [
                    {
                        img: '../assets/img/buy-comics-digital-comics.png',
                        text: 'DIGITAL COMICS'
                    },
                    {
                        img: '../assets/img/buy-comics-merchandise.png',
                        text: 'DC MERCHANDISE'
                    },
                    {
                        img: '../assets/img/buy-comics-subscriptions.png',
                        text: 'SUBSCRIPTION'
                    },
                    {
                        img: '../assets/img/buy-comics-shop-locator.png',
                        text: 'COMIC SHOP LOCATOR'
                    },
                    {
                        img: '../assets/img/buy-dc-power-visa.svg',
                        text: 'DC POWER VISA'
                    }
                ],
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
            <div v-for="label in labels">
                <img :src="getImageUrl(label.img)" alt="">
                <span>{{ label.text }}</span>
            </div>

        </div>
    </section>
</template>

<style scoped lang="scss">
@use '../style/partials/variables.scss' as *;

    section{
        background-color: $brand-primary;
    }

    .main-container{
        display: flex;
        padding: 44px;
        color: white;

        div{
            display: flex;
            align-items: center;
            margin: 0 auto;

            img{
                max-height: 55px;
                max-width: 55px;
            }
        }
    }

</style>