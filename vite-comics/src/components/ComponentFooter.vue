<script>
export default {
    name: "ComFooter"
}
</script>

<template>
    <footer>
        <section id="section-informazioni">
            <div>
                <!-- liste per contatti  -->
                <ul>
                    <li>
                        <a href="#">
                            <h3>DC COMIC</h3>
                        </a>
                    </li>
                    <li>
                        <a href="#">Characters </a>
                    </li>
                    <li>
                        <a href="#">Comics</a>
                    </li>
                    <li>
                        <a href="#"> Movies</a>
                    </li>
                    <li>
                        <a href="#"> TV</a>
                    </li>
                    <li>
                        <a href="#"> Games</a>
                    </li>
                    <li>
                        <a href="#"> News</a>
                    </li>
                    <li>
                        <a href="#">
                            <h3>SHOP</h3>
                        </a>
                    </li>
                    <li>
                        <a href="#"> Shop DC</a>
                    </li>
                    <li>
                        <a href="#">Shop DC Collectibles </a>
                    </li>
                </ul>
                <ul>
                    <li>
                        <a href="#">
                            <h3>DC</h3>
                        </a>
                    </li>
                    <li>
                        <a href="#"> Terms Of Use</a>
                    </li>
                    <li>
                        <a href="#"> Privacy policy ( Nes)</a>
                    </li>
                    <li>
                        <a href="#"> Ad Choises</a>
                    </li>
                    <li>
                        <a href="#"> Advertising</a>
                    </li>
                    <li>
                        <a href="#"> Jobs</a>
                    </li>
                    <li>
                        <a href="#"> Subscriptions</a>
                    </li>
                    <li>
                        <a href="#"> Talent Workshop</a>
                    </li>
                    <li>
                        <a href="#"> CPSC Certificates</a>
                    </li>
                    <li>
                        <a href="#"> Ratingd</a>
                    </li>
                    <li>
                        <a href="#"> Shop Help</a>
                    </li>
                    <li>
                        <a href="#"> Contact Us</a>
                    </li>
                </ul>
                <ul>
                    <li>
                        <a href="#">
                            <h3>SITES</h3>
                        </a>
                    </li>
                    <li>
                        <a href="#"> DC</a>
                    </li>
                    <li>
                        <a href="#"> MAD Magazine</a>
                    </li>
                    <li>
                        <a href="#"> DC Kids</a>
                    </li>
                    <li>
                        <a href="#"> DC Universe</a>
                    </li>
                    <li>
                        <a href="#"> DC Power Visa</a>
                    </li>
                </ul>
                <img src="../assets/img/dc-logo-bg.png" alt="">
            </div>
        </section>
        <section id="registrazione">
            <div>
                <!-- pulsante per registrarsi  -->
                <a href="" id="button-sign-up">
                    <h3>SIGN-UP NOW!</h3>
                </a>
                <!--lista con link social   -->
                <ul>
                    <li><a href="">FOLLOW US</a></li>
                    <li><img src="../assets/img/footer-facebook.png" alt=""></li>
                    <li><img src="../assets/img/footer-periscope.png" alt=""></li>
                    <li><img src="../assets/img/footer-pinterest.png" alt=""></li>
                    <li><img src="../assets/img/footer-twitter.png" alt=""></li>
                    <li><img src="../assets/img/footer-youtube.png" alt=""></li>
                </ul>
            </div>
        </section>
    </footer>
</template>

<style scoped lang="scss">
@use '../style/general.scss' as *;
@use '../style/partials/variable' as *;
// caratteristiche sezione per contattare l'azienda o domande 
#section-informazioni {
    background-image: url(../assets/img/footer-bg.jpg);
    padding: 20px 0;
    height: 350px;
    overflow: hidden;

    div {
        width: $width_blocchi ;
        margin: $margin_blocchi;
        display: $display_flex ;

        img {
            margin: -50px 0;
        }

        ul {
            margin-right: 10px;
        }
        h3{
            margin: 8px 0;
        }
    }
}
// sezione per contattare azienda sui social o registrarsi 
#registrazione {
    padding: 20px;
    background-color: #303030;

    div {
        width:$width_blocchi  ;
        margin: $margin_blocchi;
        display: $display_flex ;
        justify-content: $specific_content ;

        ul {
            display: $display_flex ;
            align-items:$specific_align ;
            li{
                margin: 0 5px;
            }
        }

        #button-sign-up {
            padding: 10px;
            border: 2px solid $color-bg;
        }

    }
}
</style>