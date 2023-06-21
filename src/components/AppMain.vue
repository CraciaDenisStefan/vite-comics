<script>
import AppCard from './AppCardBook.vue';
export default {
    components:{
      AppCard,
    },
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
            ],
            fumetti:[
                            {
                    "thumb": "https://www.coverbrowser.com/image/action-comics/1-1.jpg",
                    "price": "$19.99",
                    "series": "Action Comics",
                    "type": "comic book",
                },
                {
                    "thumb": "https://www.panini.it/media/catalog/product/cache/a5b5dd3adfe0d321084804c738f29601/M/1/M1BLLA015ISBN_0.jpg",
                    "price": "$3.99",
                    "series": "American Vampire 1976",
                    "type": "comic book",
                },
                {
                    "thumb": "https://media.wired.com/photos/593384dad80dd005b42b2817/master/w_2560%2Cc_limit/Aquaman-16.jpg",
                    "price": "$16.99",
                    "series": "Aquaman",
                    "type": "graphic novel",
                },
                {
                    "thumb": "https://d29xot63vimef3.cloudfront.net/image/batgirl/1-1.jpg",
                    "price": "$2.99",
                    "series": "Batgirl",
                    "type": "comic book",
                },
                {
                    "thumb": "https://static.posters.cz/image/750/locandine-film-in-plexiglass-batman-prowl-comic-cover-i69653.jpg",
                    "price": "$3.99",
                    "series": "Batman",
                    "type": "comic book",
                },
                {
                    "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/5/50/Batman_Beyond_v.1_1.jpg",
                    "price": "$2.99",
                    "series": "Batman Beyond",
                    "type": "comic book",
                },
                {
                    "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/0/0d/Batman_Superman_Vol_1_1.jpg",
                    "price": "$3.99",
                    "series": "Batman/Superman",
                    "type": "comic book",
                },
                {
                    "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/c/cf/Batman_Superman_Annual_Vol_2_1.jpg",
                    "price": "$4.99",
                    "series": "Batman/Superman Annual",
                    "type": "comic book",
                },
                {
                    "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/5/54/Batman_The_Joker_War_Zone_Vol_1_1.jpg",
                    "price": "$5.99",
                    "series": "Batman: The Joker War Zone",
                    "type": "comic book",
                },
                {
                    "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/6/64/Batman_Three_Jokers_Collected.jpg",
                    "price": "$6.99",
                    "series": "Batman: Three Jokers",
                    "type": "comic book",
                },
                {
                    "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/f/f8/Batman_White_Knight_Presents_Harley_Quinn_Vol_1_1.jpg",
                    "price": "$4.99",
                    "series": "Batman: White Knight Presents: Harley Quinn",
                    "type": "comic book",
                },
                {
                    "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/c/c8/Catwoman_Vol_2_1.jpg",
                    "price": "$16.99",
                    "series": "Catwoman",
                    "type": "graphic novel",
                },
            ],
        }
    }
}
</script>
<template>
    <main>
        <!-- Main parte alta vuota -->
        <div class="main_first">
            <div class="container">
                <!-- Con appcard creiamo tutte le nostre card con copertine dei fumetti -->
                <div class="content_main d_flex "> <AppCard v-for="(fumetto, index) in fumetti " :key="index" :unFumetto="fumetto"/></div>     
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
    .content_main{
        width: 100%;
        flex-wrap: wrap;
        color: white;
        padding: 40px 0;
    }
    .main_second{
        width: 100%;
        flex-wrap: wrap;
        background-color: rgb(30, 86, 206);
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
            &:hover{
            filter: invert(50%);
            cursor: pointer;
        }
        }
        .section_right{
            width: 70%;
            margin-left: 5px;
            &:hover{
            filter: invert(50%);
            cursor: pointer;
        }
    }    
    }
    img{
        width: 100%;
    }
</style>