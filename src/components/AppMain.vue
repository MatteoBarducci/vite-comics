<script>
    import Card from '../components/Card.vue';

    export default{
        name: 'AppMain',
        components: {
            Card,
        },
        data() {
            return{

            }
        }
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
            <Card></Card>
            <Card></Card>
            <Card></Card>
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
        background-color: #1C1C1C;
        color: white;
        padding: 50px;

    }


</style>