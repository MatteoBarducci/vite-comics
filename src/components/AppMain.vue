<script>
    import Card from '../components/Card.vue';

    export default{
        name: 'AppMain',
        components: {
            Card,
        },
        data() {
            return{
                cards: [
                    {
                    "thumb": "https://www.coverbrowser.com/image/action-comics/1-1.jpg",
                    "price": "$19.99",
                    "series": "Action Comics",
                    "type": "comic book"
                    },
                    {
                    "thumb": "https://www.panini.it/media/catalog/product/cache/a5b5dd3adfe0d321084804c738f29601/M/1/M1BLLA015ISBN_0.jpg",
                    "price": "$3.99",
                    "series": "American Vampire 1976",
                    "type": "comic book"
                    },
                    {
                    "thumb": "https://media.wired.com/photos/593384dad80dd005b42b2817/master/w_2560%2Cc_limit/Aquaman-16.jpg",
                    "price": "$16.99",
                    "series": "Aquaman",
                    "type": "graphic novel"
                    },
                    {
                    "thumb": "https://d29xot63vimef3.cloudfront.net/image/batgirl/1-1.jpg",
                    "price": "$2.99",
                    "series": "Batgirl",
                    "type": "comic book"
                    },
                    {
                    "thumb": "https://static.posters.cz/image/750/locandine-film-in-plexiglass-batman-prowl-comic-cover-i69653.jpg",
                    "price": "$3.99",
                    "series": "Batman",
                    "type": "comic book"
                    },
                    {
                    "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/5/50/Batman_Beyond_v.1_1.jpg/revision/latest?cb=20080809201655",
                    "price": "$2.99",
                    "series": "Batman Beyond",
                    "type": "comic book"
                    },
                    {
                    "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/0/0d/Batman_Superman_Vol_1_1.jpg/revision/latest/scale-to-width-down/1200?cb=20130627211607",
                    "price": "$3.99",
                    "series": "Batman/Superman",
                    "type": "comic book"
                    },
                    {
                    "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/c/cf/Batman_Superman_Annual_Vol_2_1.jpg/revision/latest?cb=20200929145132",
                    "price": "$4.99",
                    "series": "Batman/Superman Annual",
                    "type": "comic book"
                    },
                    {
                    "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/5/54/Batman_The_Joker_War_Zone_Vol_1_1.jpg/revision/latest?cb=20200929124651",
                    "price": "$5.99",
                    "series": "Batman: The Joker War Zone",
                    "type": "comic book"
                    },
                    {
                    "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/6/64/Batman_Three_Jokers_Collected.jpg/revision/latest?cb=20201123054610",
                    "price": "$6.99",
                    "series": "Batman: Three Jokers",
                    "type": "comic book"
                    },
                    {
                    "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/f/f8/Batman_White_Knight_Presents_Harley_Quinn_Vol_1_1.jpg/revision/latest?cb=20201124094800",
                    "price": "$4.99",
                    "series": "Batman: White Knight Presents: Harley Quinn",
                    "type": "comic book"
                    },
                    {
                    "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/c/c8/Catwoman_Vol_2_1.jpg/revision/latest?cb=20160303223223",
                    "price": "$16.99",
                    "series": "Catwoman",
                    "type": "graphic novel"
                    }
                ],
            }
        }, 
    }
</script>

<template>
    <section>
        <div class="main-container">
            <button><h2>CURRENT SERIES</h2></button>
        </div>
    </section>
    <main>
        <div class="main-container">
            <div class="card-container">
                <Card v-for="card in cards" :text="card.series" :image="card.thumb"></Card>

            </div>
            <div class="button-container">
                <button><h4>LOAD MORE</h4></button>
            </div>
        </div>
    </main>
</template>

<style scoped lang="scss">
@use '../style/partials/variables.scss' as *;

    section{
        height: 400px;
        background-image: url(../assets/img/jumbotron.jpg);
        background-size: cover;
        background-repeat: no-repeat;
        position: relative;

        button{
            padding: 18px 25px;
            background-color: $brand-primary;
            color: white;
            border: none;
            position: absolute;
            bottom: -25px;
        }
    }

    main{
        padding-top: 20px;
        background-color: #1C1C1C;
        color: white;
        padding: 50px;
        .card-container{
            padding: 10px;
            display: flex;
            flex-wrap: wrap;
            flex-grow: 0;
            gap: 20px;
            justify-content: space-evenly;
        }

        .button-container{
            display: flex;
            justify-content: center;
            margin-top: 35px;
        }

        button{
            padding: 18px 25px;
            background-color: $brand-primary;
            color: white;
            border: none;
        }
    }


</style>