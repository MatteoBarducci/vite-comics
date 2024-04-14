<script>
    export default{
        name: 'Card',
        props: ['image', 'text'],
        data() {
            return{

            }
        }
    }
</script>

<template>
    <div class="card">
        <img :src="image" >
        <figcaption>{{ text }}</figcaption>
        
    </div>
</template>

<style scoped lang="scss">
@use '../style/partials/variables.scss' as *;

    .card{
        width: 15%; 
        
        img{
            width: 100%;
            height: 189px;
            object-fit: cover;

        }
        figcaption{
            margin-top: 15px;
            margin-bottom: 10px;
        }
    }

</style>