<template>
    <footer>
        <div class="footer-top">
            <div class="container">
                <!-- Row -->
                <div class="row">
                    <!-- Column -->
                    <div class="col">
                        <h2>DC Comics</h2>
                        <ul>
                            <li><a href="#">Characters</a></li>
                            <li><a href="#">Comics</a></li>
                            <li><a href="#">Movies</a></li>
                            <li><a href="#">TV</a></li>
                            <li><a href="#">Games</a></li>
                            <li><a href="#">Videos</a></li>
                            <li><a href="#">News</a></li>
                        </ul>
                        
                        <h2>DC Shop</h2>
                        <ul>
                            <li><a href="#">Shop DC</a></li>
                            <li><a href="#">Shop DC Collectibles</a></li>
                        </ul>
                    </div>

                    <!-- Column -->
                    <div class="col">
                        <h2>DC</h2>

                        <ul>
                            <li><a href="#">Terms Of Use</a></li>
                            <li><a href="#">Privacy Policy (New)</a></li>
                            <li><a href="#">Advertising</a></li>
                            <li><a href="#">Jobs</a></li>
                            <li><a href="#">Subscriptions</a></li>
                            <li><a href="#">CPSC Certificates</a></li>
                            <li><a href="#">Ratings</a></li>
                            <li><a href="#">Shop Help</a></li>
                            <li><a href="#">Contact Us</a></li>
                        </ul>
                    </div>

                    <!-- Column -->
                    <div class="col">
                        <h2>Sites</h2>

                        <ul>
                            <li><a href="#">DC</a></li>
                            <li><a href="#">DC UNIVERSE INFINITE</a></li>
                            <li><a href="#">DC Kids</a></li>
                            <li><a href="#">DC Shop</a></li>
                            <li><a href="#">MAD Magazine</a></li>
                        </ul>
                    </div>

                    <!-- Column -->
                    <p>All Site Content TM and © 2020 DC Entertainment, unless otherwise <a href="#">noted here</a>. All rights reserved. <a href="#">Cookies Settings</a></p>
                </div>
            </div>

            <!-- Logo DC -->
            <!-- <img src="../assets/img/dc-logo-bg.png" alt="logo DC"> -->
        </div>
    </footer>
</template>


<script>
export default {
    name: 'MyFooter'
}
</script>


<style lang="scss" scoped>
@import '../styles/variables';

footer {
    
    .footer-top {
        background-image: url(../assets/img/dc-logo-bg.png), url(../assets/img/footer-bg.jpg);
        background-size: auto, cover;
        background-position: center right, center;
        background-repeat: no-repeat;
        padding: 3rem 0;
        color: $brand_tertiary_color;
        
        .container {

            .row {
                display: flex;
                flex-wrap: wrap;
                width: 50%;

                .col {
                margin-right: 2rem;
                width: 6rem;
                flex-shrink: 0;

                    h2 {
                        font-size: 1.1rem;    
                        color: white;
                        font-weight: 800;
                        text-transform: uppercase;
                        margin-bottom: 0.5rem;
                    }
                    ul {
                        margin-bottom: 1rem;

                        
                    }
                }
                li:hover {
                    color: $brand_primary_color;
                }
                li, p {
                    font-size: 0.75rem;
                    line-height: 1.2rem;
                    font-weight: 600;
                }
                p {
                    display: block;

                    a {
                        color: $brand_primary_color;
                    }
                }
            }
        }
    }
}

</style>
