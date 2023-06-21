<script>
export default {
    props:{
        unFumetto: Object
    }
}
</script>
<template >
    <div class="card">
        <img :src="unFumetto.thumb" alt="">
        <div class="title_card">
            <h5>{{ unFumetto.series }}</h5>
        </div>    
    </div>
</template>
<style lang="scss" scoped>
@use '../styles/partials/variables'as *;
.card{
    width: calc(100% / 6 - 20px);
    margin: 10px;
    cursor: pointer;

    &:hover{
    filter:sepia(100%);
}
    .title_card{
        text-transform: uppercase;
    }
    img{
    width: 100%;
    height: 150px;
    object-fit: cover;
    object-position: top;
    margin-bottom: 10px;
}

}
</style>