<template>
    <section class="shop">
        <div class="container">
            <!-- Shop List -->
            <ul>
                <!-- <li v-for="listItem, index in shopListItems" :key="index">
                    <a :href="listItem.url">
                        <img :src="`../assets/img/${listItem.image}`" alt="">
                        <span class="text">{{listItem.text}}</span>
                    </a>
                </li> -->
                <li>
                    <a href="#">
                        <img src="../assets/img/buy-comics-digital-comics.png" alt="">
                        <span class="text">Digital Comics</span>
                    </a>
                </li>
                <li>
                <li>
                    <a href="#">
                        <img src="../assets/img/buy-comics-merchandise.png" alt="">
                        <span class="text">DC Merchandise</span>
                    </a>
                </li>
                <li>
                    <a href="#">
                        <img src="../assets/img/buy-comics-subscriptions.png" alt="">
                        <span class="text">Subscription</span>
                    </a>
                </li>
                <li>
                    <a href="#">
                        <img src="../assets/img/buy-comics-shop-locator.png" alt="">
                        <span class="text">Comic Shop Locator</span>
                    </a>
                </li>
                <li>
                    <a href="#">
                        <img src="../assets/img/buy-dc-power-visa.svg" alt="">
                        <span class="text">DC Power Visa</span>
                    </a>
                </li>
            </ul>
        </div>
    </section>
</template>


<script>
export default {
    name: 'SectionShop',
    data() {
        return {
            shopListItems: [
                {
                    text: 'Digital Comics',
                    image: 'buy-comics-digital-comics.png',
                    url: '#'
                },
                {
                    text: 'DC Merchandise',
                    image: 'buy-comics-merchandise.png',
                    url: '#'
                },
                {
                    text: 'Subscription',
                    image: 'buy-comics-subscriptions.png',
                    url: '#'
                },
                {
                    text: 'Comic Shop Locator',
                    image: 'buy-comics-shop-locator.png',
                    url: '#'
                },
                {
                    text: 'DC Power Visa',
                    image: 'buy-dc-power-visa.svg',
                    url: '#'
                },
            ]
        }
    }
}
</script>


<style lang="scss" scoped>
@import '../styles/variables';

section {
    padding: 3rem 0;
    background-color: $brand_primary_color;

    ul {
        display: flex;
        justify-content: space-around;
        align-items: center;
    }

    img {
        vertical-align: middle;
        width: 2.5rem;
        margin-right: 1rem;    
    }
    .text {
        vertical-align: middle;
        color: white;
        font-weight: 400;
        text-transform: uppercase;
        font-size: 0.85rem;
    }
}

</style>
