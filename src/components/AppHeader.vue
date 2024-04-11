<script>
    export default{
        name: 'AppHeader',
        data() {
            return{
                links: [
                    {
                        text: 'CHARACTERS',
                        active: false
                    },
                    {
                        text: 'COMICS',
                        active: true
                    },
                    {
                        text: 'MOVIES',
                        active: false
                    },
                    {
                        text: 'TV',
                        active: false
                    },
                    {
                        text: 'GAMES',
                        active: false
                    },
                    {
                        text: 'COLLECTIBLES',
                        active: false
                    },
                    {
                        text: 'VIDEOS',
                        active: false
                    },
                    {
                        text: 'FANS',
                        active: false
                    },
                    {
                        text: 'NEWS',
                        active: false
                    },
                    {
                        text: 'SHOP',
                        active: false
                    },
                ],
            }
        }
    }
</script>

<template>
    <header>
        <div class="main-container">
            <div class="header-left">
                <img src="../assets/img/dc-logo.png" alt="Logo">
            </div>
            <nav class="header-right">
                <ul>
                    <li v-for="link in links" >
                        <a href="#" :class="{'active': link.active}">{{ link.text }}</a>
                    </li>
                </ul>
            </nav>
        </div>
    </header>
</template>

<style scoped lang="scss">
@use '../style/partials/variables.scss' as *;

    header{
        background-color: white;
        padding: 20px;

        .main-container{
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        ul{
            display: flex;
            gap: 30px;

            .active{
                color: $brand-primary; 
            }
        }
    }
</style>