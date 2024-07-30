<script>
export default {
    
}
</script>
<template>
    <footer>
        <div class="topFooter">
            <div class="container">
                <div class="row">
                    <div class="topfooterright">           
                        <div class="w-50 p-4">
                            <div class="row">
                                <div class="col-4">
                                    <p class="footerTitle m-0">DC COMICS</p>
                                    <ul class="list-unstyled mt-2">
                                        <li><a href="#">Charachters</a></li>
                                        <li><a href="#">Comics</a></li>
                                        <li><a href="#">Movies</a></li>
                                        <li><a href="#">TV</a></li>
                                        <li><a href="#">Games</a></li>
                                        <li><a href="#">Videos</a></li>
                                        <li><a href="#">News</a></li>
                                    </ul>
                                    <p class="footerTitle m-0">SHOP</p>
                                    <ul class="list-unstyled mt-2">
                                        <li><a href="#">Shop DC</a></li>
                                        <li><a href="#">Shop DC Collectibles</a></li>
                                    </ul>
                                </div>
                                <div class="col-4">
                                    <p class="footerTitle m-0">DC</p>
                                    <ul class="list-unstyled mt-2">
                                        <li><a href="#">Terms Of Use</a></li>
                                        <li><a href="#">Privacy policy (new)</a></li>
                                        <li><a href="#">Ad Choices</a></li>
                                        <li><a href="#">Advertising</a></li>
                                        <li><a href="#">Jobs</a></li>
                                        <li><a href="#">Subscriptions</a></li>
                                        <li><a href="#">Talent Workshop</a></li>
                                        <li><a href="#">CPSC Certificates</a></li>
                                        <li><a href="#">Ratings</a></li>
                                        <li><a href="#">Shop Help</a></li>
                                        <li><a href="#">Contact Us</a></li>
        
                                    </ul>
                                </div>
                                <div class="col-4">
                                    <p class="footerTitle m-0">SITES</p>
                                    <ul class="list-unstyled mt-2">
                                        <li><a href="#">DC</a></li>
                                        <li><a href="#">MAD magazine</a></li>
                                        <li><a href="#">DC kids</a></li>
                                        <li><a href="#">DC Universe</a></li>
                                        <li><a href="#">DC Power Visa</a></li>
                                    </ul>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
        <div class="bottomFooter">
            <div class="container">
                <div class="row">
                    <div class="col-3">
                        <button class="btnFooter">SIGN UP NOW!</button>
                    </div>
                    <div class="col-9 d-flex align-items-center justify-content-end">
                        <p class="ctaFooter m-0">FOLLOW US</p>
                        <div class="icons">
                            <a href="#" class="iconSocial">
                                <img src="/public/footer-facebook.png" alt="">
                            </a>
                            <a href="#" class="iconSocial">
                                <img src="/public/footer-twitter.png" alt="">
                            </a>
                            <a href="#" class="iconSocial">
                                <img src="/public/footer-youtube.png" alt="">
                            </a>
                            <a href="#" class="iconSocial">
                                <img src="/public/footer-pinterest.png" alt="">
                            </a>
                            <a href="#" class="iconSocial">
                                <img src="/public/footer-periscope.png" alt="">
                            </a>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </footer>
</template>
<style lang="scss" scoped>
    .topFooter{
        background-image: url('/footer-bg.jpg');
        background-repeat: no-repeat;
        background-size: cover;
        position: relative;
        overflow: hidden;
    }
    .topfooterright{
        background-image: url('/dc-logo-bg.png');
        background-repeat: no-repeat;
        background-position: right;
        background-size: 400px;
        
    }
    .bottomFooter{
        background-color: #303030;
        height: 75px;
        display: flex;
        align-items: center;
        justify-content: center;

        img{
            width: 20px;
            margin: 10px;
        }
    }
    .footerTitle{
        color: #fff;
        font-weight: 600;
        font-size: 0.75rem;
    }
    li{
        font-size: 0.6rem;

        a{
            text-decoration: none;
            color: #999999;
            transition: all 0.25s;
        }
        a:hover{
            color: #0081F8;
        }
    }
    .decorationLogo{
        position: absolute;
        z-index: 1;
        width: 34vw;
        max-width: 500px;
        top: -25%;
        right: -10px;
    }
    .btnFooter{
        border: 1px solid #0081F8;
        background-color:transparent ;
        padding: 5px;
        font-size: 0.6rem;
        font-weight: 600;
        color: #fff; 
        transition: all 0.5s;
    }
    .btnFooter:hover{
        background-color:#0081F8 ;
    }
    .ctaFooter{
        color: #0081F8;
        font-size: 0.75rem;
        font-weight: 700;
    }
    .iconSocial{
        transition: all 0.2s;
    }
    .iconSocial:hover{
        filter: brightness(0) saturate(100%) invert(100%) sepia(0%) saturate(7441%) hue-rotate(51deg) brightness(116%) contrast(93%);
    }

</style>