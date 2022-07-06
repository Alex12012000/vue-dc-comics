<template>
    
    <!-- Footer -->
   <footer>
        <div class="up-footer">
            <div class="container">
                <div class="left-side">
                    <div class="first-ul">
                        <h3>DC COMICS</h3>
                        <ul>
                            <li>
                                <a href="#">Characters</a>
                            </li>
                            <li>
                                <a href="#">Comics</a>
                            </li>
                            <li>
                                <a href="#">Movies</a>
                            </li>   
                            <li>
                                <a href="#">TV</a>
                            </li>          
                            <li>
                                <a href="#">Games</a>
                            </li>   
                            <li>
                                <a href="#">News</a>
                            </li>   
                        </ul>
                        <h3>SHOP</h3>
                        <ul>
                            <li>
                                <a href="#">Shop DC</a>
                            </li>
                            <li>
                                <a href="#">Shop DC collectibles</a>
                            </li>
                        </ul>
                    </div>
                    <div class="second-ul">
                        <h3>DC</h3>
                        <ul>
                            <li>
                                <a href="#">Terms Of Use</a>
                            </li>
                            <li>
                                <a href="#">Privacy policy(new)</a>
                            </li>
                            <li>
                                <a href="#">Ad Choices</a>
                            </li>
                            <li>
                                <a href="#">Advertsing</a>
                            </li>
                            <li>
                                <a href="#">Jobs</a>
                            </li>
                            <li>
                                <a href="#">Subscriptions</a>
                            </li>
                            <li>
                                <a href="#">Talent Workshop</a>
                            </li>
                            <li>
                                <a href="#">CPSC Certifications</a>
                            </li>
                            <li>
                                <a href="#">Ratings</a>
                            </li>
                            <li>
                                <a href="#">Shop Help</a>
                            </li>
                            <li>
                                <a href="#">Contact US</a>
                            </li>
                        </ul>
                    </div>
                    <div class="third-ul">
                        <h3>SITES</h3>
                        <ul>
                            <li>
                                <a href="#">DC</a>
                            </li>
                            <li>
                                <a href="#">MAD Magazine</a>
                            </li>
                            <li>
                                <a href="#">DC Kids</a>
                            </li>
                            <li>
                                <a href="#">DC Universe</a>
                            </li>
                            <li>
                                <a href="#">DC Power Visa</a>
                            </li>
                        </ul>
                    </div>
                </div>
                <div class="right-side">
                    <img src="../assets/img/dc-logo-bg.png" alt="">
                </div>
            </div>
        </div>

        <div class="bottom-footer">
            <div class="container">
                <div class="contents">
                    <div class="btn">
                        <a href="#">SIGN-UP NOW!</a>
                    </div>
                    <div class="socials">
                        <span>FOLLOW US</span>
                        <div class="icon">
                            <a href="#">
                                <img src="../assets/img/footer-facebook.png">
                            </a>
                            <a href="#">
                                <img src="../assets/img/footer-twitter.png">
                            </a>
                            <a href="#">
                                <img src="../assets/img/footer-youtube.png">
                            </a>
                            <a href="#">
                                <img src="../assets/img/footer-pinterest.png">
                            </a>
                            <a href="#">
                                <img src="../assets/img/footer-periscope.png">
                            </a>
                        </div>
                    </div>
                </div>
            </div>
        </div>
   </footer>

</template>


<script>
export default {
    name: "PageFooter",
}
</script>


<style lang="scss" scoped>
@import "../style/common.scss";
@import "../style/variables.scss";

.up-footer {
    background-image: url('../assets/img/footer-bg.jpg');
    height: 400px;
    display: flex;
    justify-content: space-between;
    align-items: center;
    position: relative;

    .left-side {
        display: flex;
        div {
            margin: 5px 10px;
            color: white;
        }
        ul {
            padding: 20px 0;

            li {

                margin: 5px 0;
                a {
                color: grey;
            }
            }
        }
    }

    .right-side {
        position: absolute;
        bottom: -40px;
        right: 150px;

        img {
            width: 500px;

        }
    }
}

.bottom-footer {
    height: 100px;
    background-color: #303030;
    position: relative;
    z-index: 1;
    display: flex;
    align-items: center;

    .contents {
        display: flex;
        align-items: center;
        justify-content: space-between; 
    }
 
    .btn {
        padding: 10px;
        border: 1px solid $main_color;

        a {
            color: white;
        }
    }

    .socials {
        display: flex;
        align-items: center;

        .icon {
            display: flex;

            a {
                margin: 0 5px;
                width: 30px;
            }
        }

        span {
            color: $main_color;
            margin: 0 5px;
        }
    }
}

</style>