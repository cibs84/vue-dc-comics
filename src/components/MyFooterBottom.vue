<template>
    <div class="footer-bottom">
        <div class="container">

            <!-- Signup -->
            <div class="signup">
                <button>SIGN-UP NOW!</button>
            </div>

            <!-- Socials Menu -->
            <nav>
                <h2>FOLLOW US</h2>

                <ul class="main-menu">
                    <li>
                        <img src="../assets/img/footer-facebook.png" alt="">
                    </li> 
                    <li>
                        <img src="../assets/img/footer-twitter.png" alt="">
                    </li> 
                    <li>
                        <img src="../assets/img/footer-youtube.png" alt="">
                    </li> 
                    <li>
                        <img src="../assets/img/footer-pinterest.png" alt="">
                    </li> 
                    <li>
                        <img src="../assets/img/footer-periscope.png" alt="">
                    </li> 
                </ul>
            </nav>
        </div>
    </div>
</template>


<script>
export default {
    name: 'MyFooterBottom',
}
</script>


<style lang="scss" scoped>
@import '../styles/variables';

.footer-bottom {
    padding: 2rem 0;
    background-color: $brand_secondary_color;

    .container {
        display: flex;
        justify-content: space-between;
        align-items: center;
    
        .signup {
            flex-grow: 1;
    
            button {
                color: white;
                text-transform: uppercase;
                border: 2px solid $brand_primary_color;
                background-color: transparent;
                padding: 1rem;
                font-size: 1rem;
                cursor: pointer;
            }
        }
        nav {
            display: flex;
            align-items: center;

            h2 {
                color: $brand_primary_color;
                text-transform: uppercase;
            }

            .main-menu {
                display: flex;
        
                li {
                    margin-left: 1rem;

                    img {
                        margin-top: 0.3rem;
                        cursor: pointer;
                    }
                }
            }
        }
    }
}
</style>