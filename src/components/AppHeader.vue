<script>
export default {
    data(){
        return{
            menu:[
                {
                    label:'Characters',
                    link:'#',
                    active: false,
                },
                {
                    label:'Comics',
                    link:'#',
                    active: false,
                },
                {
                    label:'Movies',
                    link:'#',
                    active: false,
                },
                {
                    label:'Tv',
                    link:'#',
                    active: false,
                },
                {
                    label:'Games',
                    link:'#',
                    active: false,
                },
                {
                    label:'Collectibles',
                    link:'#',
                    active: false,
                },
                {
                    label:'Videos',
                    link:'#',
                    active: false,
                },
                {
                    label:'Fans',
                    link:'#',
                    active: false,
                },
                {
                    label:'News',
                    link:'#',
                    active: false,
                },
                {
                    label:'Shop',
                    link:'#',
                    active: false,
                },
            ]
        }
    }
    
}
</script>
<template>
   <header class="container d_flex">
    <!-- Container con dentro logo e menu  -->
    <div class="logo">
        <img src="../assets/img/dc-logo.png" alt="">
    </div>
    <div class="menu">
        <ul class="d_flex menu_header">
            <li v-for="(lista, index) in menu" :key="index">
               <a :href="lista.link"> {{ lista.label }}</a>
            </li>
        </ul>
        <div class="hamburgher_menu">
            <i class="fa-solid fa-bars"></i>
        </div>
    </div>
   </header>
</template>
<style scoped lang="scss">
@use '../styles/partials/variables'as *;
    header{
        justify-content: space-between;
        align-items: center;
    }
    img{
        width: 4rem;
    }
    ul{
        list-style: none;
        vertical-align: bottom;
        li{
            padding: 40px 0;
            margin: 0 0.5rem;
            font-size: 0.8rem;
            border-bottom:5px solid white ;
            
            a{
                text-decoration: none;
                font-weight: 700;
                text-transform: uppercase;
                color:rgb(70, 70, 70);
                &:hover{
                color: $dc_color;
               
            }

            }
            &:hover{
                border-bottom: 5px solid $dc_color;
               
            }
        }
    }
    .hamburgher_menu{
            display: none;
            .fa-solid{
                color: rgb(70, 70, 70);
                font-size: 2rem;
                padding: 30px 0;
                cursor: pointer;
                &:hover{
                    color: $dc_color;
                }
            }
            
        }
    @media screen and (max-width: 1068px){
        .menu_header{
            display: none;
        }
        .hamburgher_menu{
            display: block;
        }
    }
</style>