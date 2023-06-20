<script>
export default {
    data(){
        return{
            menu_main:[
                {
                    img:'./assets/img/buy-comics-digital-comics.png',
                    describtion:'Digital comics',
                },
                {
                    img:'./assets/img/buy-comics-merchandise.png',
                    describtion:'Dc merchandise',
                },
                {
                    img:'./assets/img/buy-comics-subscriptions.png',
                    describtion:'Subscribtion',
                },
                {
                    img:'./assets/img/buy-comics-shop-locator.png',
                    describtion:'Comic shop locador',
                },
                {
                    img:'./assets/img/buy-dc-power-visa.svg',
                    describtion:'Dc power visa',
                },
            ]
        }
    }
}
</script>
<template>
    <main>
        <!-- Main parte alta vuota -->
        <div class="main_first">

            <div class="container">
                <h2 class="content_main"> Content goes here </h2>
            </div>

        </div>
        <!-- Inizio main sezione sotto -->
        <div class="main_second">
            <div class="main_second_section container d_flex">
                <div class="section d_flex " v-for="(menu, index) in menu_main " :key="index"> 
                    <div class="section_left">
                        <img :src="menu.img" alt="">
                    </div>   
                    <div class="section_right">
                        {{ menu.describtion }}
                    </div>
                </div>
            </div>
        </div>
    </main>
</template>
<style scoped lang="scss">
    .main_first{
        width: 100%;
        background-color: rgb(27, 27, 27);
    }
    .main_second{
        width: 100%;
        background-color: rgb(30, 86, 206);
        .main_second_section{
            justify-content: center;
        }
    }
    .section{
        width: calc(100% / 5 - 40px);
        margin: 0 20px;
        font-size: 0.8rem;
        align-items: center;
        font-weight: 700;
        text-transform: uppercase;
        color: white;
        padding: 40px 0;
        .section_left{
            width: 20%;
        }
        .section_right{
            width: 70%;
            margin-left: 5px;
        }
    }
    img{
        width: 100%;
       
    }


    .content_main{
        color: white;
        padding: 40px 0;
    }
</style>