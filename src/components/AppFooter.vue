<script>
export default {
    
}
</script>

<template>
    <footer>
        <!-- Footer parte alta  -->
        <div class="footer_up">
            <div class="container d_flex container_logo_info">
                <div class="info_footer d_flex">
                    <div class="li_footer">
                        <div class="li_footer_up">
                            <ul>
                                <h4>DC COMICS</h4>
                                <li><a href="#">Characters</a></li>
                                <li><a href="#">Comics</a></li>
                                <li><a href="#">Movies</a></li>
                                <li><a href="#">TV</a></li>
                                <li><a href="#">Games</a></li>
                                <li><a href="#">Videos</a></li>
                                <li><a href="#">News</a></li>
                            </ul>
                        </div>
                        <div class="li_footer_down">
                            <ul>
                                <h4>SHOP</h4>
                                <li><a href="#">Shop DC</a></li>
                                <li><a href="#">Shop DC Colectibles </a></li>
                            </ul>
                        </div>
                    </div>
                    <div class="li_footer">
                        <ul>
                                <h4>DC</h4>
                                <li><a href="#">Terms Of Use</a></li>
                                <li><a href="#">Privacy policy(New)</a></li>
                                <li><a href="#">Ad Choices</a></li>
                                <li><a href="#">Advertising</a></li>
                                <li><a href="#">Jobs</a></li>
                                <li><a href="#">Subscriptions</a></li>
                                <li><a href="#">Talent Workshops</a></li>
                                <li><a href="#">CPSC Certificates</a></li>
                                <li><a href="#">Ratings</a></li>
                                <li><a href="#">Shop Help</a></li>
                                <li><a href="#">Contact Us</a></li>
                            </ul>
                    </div>
                    <div class="li_footer">
                        <ul>
                                <h4>SITES</h4>
                                <li><a href="#">DC</a></li>
                                <li><a href="#">MAD Magazine</a></li>
                                <li><a href="#">DC Kids</a></li>
                                <li><a href="#">DC Univers</a></li>
                                <li><a href="#">DC Power Visa</a></li>
                            </ul>
                    </div>
                </div>
                <div class="logo_footer">
                    
                </div>
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
    .container_logo_info{
        justify-content: space-between;
    }
    .info_footer{
        width: 40%;
        padding: 30px 0;
    }
    .logo_footer{
        width: 40%;
        background-image: url(../assets/img/dc-logo-bg.png);
        background-size: cover;
        background-position-y: center;
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
       color: white;
        margin: 5px;
    }
    ul{
        list-style: none;
        a{
                text-decoration: none;
                color: rgb(153, 151, 151);
    
            }
       }
    .li_footer_down{
        margin-top: 20px;
    }
    h4{
        margin-bottom: 10px;
    }
        
</style>