<script>
export default {
    data(){
        return{
            menu_main:[
                {
                    img:'../assets/img/buy-comics-digital-comics.png',
                    describtion:'Digital comics',
                },
                {
                    img:'../assets/img/buy-comics-merchandise.png',
                    describtion:'Dc merchandise',
                },

            ]
        }
    }
}
</script>
<template>
    <main>
        <div class="main_first"></div>
        <!-- Inizio main sezione sotto -->
        <div class="main_second">
            <div class="main_second_section container d_flex">
                <div class="section " v-for="(menu, index) in menu_main " :key="index">    
                    <div class="section_right">
                        <img :src="menu.img" alt="">
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
        height: 100px;
        background-color: black;
    }
    .main_second{
        width: 100%;
        height: 100px;
        background-color: blue;
        .main_second_section{
            justify-content: center;
        }
    }
    .section{
        margin: 0 20px;
    }
    img{
        width: 50px;
        height: 50px;
    }
</style>