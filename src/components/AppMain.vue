<script>
export default {
    
}
</script>
<template>
    <main>
        <div class="main_first"></div>
        <!-- Inizio main sezione sotto -->
        <div class="main_second">
            <div class="main_second_section container d_flex">
                <div class="section ">
                    <div class="section_left"></div>
                    <div class="section_right"></div>
                </div>
                <div class="section ">
                    <div class="section_left"></div>
                    <div class="section_right"></div>
                </div>
                <div class="section">
                    <div class="section_left"></div>
                    <div class="section_right"></div>
                </div>
                <div class="section">
                    <div class="section_left"></div>
                    <div class="section_right"></div>
                </div>
                <div class="section">
                    <div class="section_left"></div>
                    <div class="section_right"></div>
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
        .section_left, .section_right{
            width: 100px;
            height: 50px;
            background-color: green;
        }
    }
</style>