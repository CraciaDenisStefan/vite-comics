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
        <ul class="d_flex">
            <li v-for="(lista, index) in menu" :key="index">
               <a :href="lista.link"> {{ lista.label }}</a>
            </li>
        </ul>
    </div>
   </header>
</template>
<style scoped lang="scss">
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
                color: rgb(42, 86, 228);
               
            }

            }
            &:hover{
                border-bottom: 5px solid rgb(42, 86, 228);
               
            }
        }
    }
</style>