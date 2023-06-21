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
                        <!-- div con dentro due liste una sopra l'altra -->
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
                    <!-- Altri due div con le liste di info nel footer parte alta -->
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
                    <!-- Div per sistemare il logo dc come background -->
                </div>
            </div>
        </div>
        <!-- Footer parte bassa -->
        <div class="footer_down">
            <div class="container d_flex social_footer_down">
                <!-- Bottone per il sing up -->
                <div class="button_footer">
                    <button>SIGN-UP NOW!</button>
                </div>
                <div class="social_footer">
                    <!-- Lista social media footer -->
                    <ul class="d_flex">
                        <li class="follow"> FOLLOW US </li>
                        <li> <a href="#"><img src="../assets/img/footer-facebook.png" alt=""></a></li>
                        <li> <a href="#"><img src="../assets/img/footer-twitter.png" alt=""></a></li>
                        <li> <a href="#"><img src="../assets/img/footer-youtube.png" alt=""></a></li>
                        <li> <a href="#"><img src="../assets/img/footer-pinterest.png" alt=""></a></li>
                        <li> <a href="#"><img src="../assets/img/footer-periscope.png" alt=""></a></li>
                    </ul>
                </div>

            </div>
        </div>
    </footer>
</template>

<style scoped lang="scss">
@use '../styles/partials/variables'as *;
    .footer_up{
        width: 100%;
        background-image: url(../assets/img/footer-bg.jpg); 
    }
    .container_logo_info{
        justify-content: space-between;
    }
    .info_footer{
        width: 50%;
        padding: 30px 0;
        
    }
    .logo_footer{
        width: 50%;
        background-image: url(../assets/img/dc-logo-bg.png);
        background-size: cover;
        background-position-y: center;
    }
    .footer_down{
        width: 100%;
        background-color: rgb(23, 23, 24);

        .social_footer_down{
            justify-content: space-between;
            align-content: center;

            .button_footer, .social_footer{
                margin: 30px 0;
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
                &:hover{
                    color: white;
                }
            }
       }
    .li_footer_down{
        margin-top: 20px;
    }
    h4{
        margin-bottom: 10px;
    }

    // FOOTER PARTE SOTTO
    button{
        border: 2px solid $dc_color;
        background: transparent;
        color: white;
        padding: 15px;
        font-weight: 700;
        font-size: 1rem;
        cursor: pointer;
        &:hover{
                background-color: $dc_color;
        }
    }
    .social_footer{
        a{
            margin: 0 10px;
            &:hover{
                filter: invert(100%);
        }
        }
        
    }
    .follow{
       align-self: center;
       color: $dc_color;
       font-weight: 700;
       margin-right: 10px;
       cursor: context-menu;
    }



@media screen and (max-width: 1068px){
    .info_footer{
        width: 70%;
    }
    .logo_footer{
        width: 30%;
        background-size: contain;
        background-repeat: no-repeat;}
}

@media screen and (max-width: 860px){
    .logo_footer{
        display: none;
    }
    .info_footer{
        width: 100%;
        flex-wrap: wrap;
    }
   
}
@media screen and (max-width: 760px){
    .social_footer_down{
        flex-wrap: wrap;
    }
   
}
@media screen and (max-width: 540px){
   .follow{
    display: none;
   }
}
        
</style>