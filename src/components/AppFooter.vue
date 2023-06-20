<script>
export default {
    
}
</script>

<template>
    <footer>
        <!-- Footer parte alta  -->
        <div class="footer_up">
            <div class="container d_flex">
                <div class="info_footer d_flex">
                    <div class="li_footer">
                        <div class="li_footer_up"></div>
                        <div class="li_footer_down"></div>
                    </div>
                    <div class="li_footer"></div>
                    <div class="li_footer"></div>
                </div>
                <div class="logo_footer"></div>
            </div>
        </div>
        <!-- Footer parte bassa -->
        <div class="footer_down">
            <div class="container d_flex social_footer_down">
                <div class="button_footer"></div>
                <div class="social_footer">
                    <ul>
                        <li> <a href="#"></a></li>
                        <li> <a href="#"></a></li>
                        <li> <a href="#"></a></li>
                        <li> <a href="#"></a></li>
                        <li> <a href="#"></a></li>
                        <li> <a href="#"></a></li>
                    </ul>
                </div>

            </div>
        </div>
    </footer>
</template>

<style scoped lang="scss">
    .footer_up{
        width: 100%;
        background-image: url(../assets/img/footer-bg.jpg); 
    }
    .info_footer{
        width: 40%;
    }
    .logo_footer{
        width: 60%;
    }
    .footer_down{
        width: 100%;
        height: 100px;
        background-color: rgb(23, 23, 24);

        .social_footer_down{
            justify-content: space-between;

            .button_footer, .social_footer{
                width: 200px;
                height: 50px;
                background-color: yellow;
                margin: 20px 0;
            }
        }
    }
    .li_footer{
        width: 50px;
        height: 100px;
        background-color: yellow;
        margin: 5px;
        
        .li_footer_up, .li_footer_down{
            width: 20px;
            height: 50px;
            background-color: red;
            border: 1px solid black;
        }
    }
    
</style>