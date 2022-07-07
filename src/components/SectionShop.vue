<template>
    <section class=shop>
        <div class=container>
            <!-- Shop List -->
            <ul>
                <li v-for="(listItem, index) in shopListItems" :key=index>
                    <a :href=listItem.url>
                        <img :src="listItem.image" />
                        <span class=text>{{listItem.text}}</span>
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
                    image: require('../assets/img/buy-comics-digital-comics.png'),
                    url: '#'
                },
                {
                    text: 'DC Merchandise',
                    image: require('../assets/img/buy-comics-merchandise.png'),
                    url: '#'
                },
                {
                    text: 'Subscription',
                    image: require('../assets/img/buy-comics-subscriptions.png'),
                    url: '#'
                },
                {
                    text: 'Comic Shop Locator',
                    image: require('../assets/img/buy-comics-shop-locator.png'),
                    url: '#'
                },
                {
                    text: 'DC Power Visa',
                    image: require('../assets/img/buy-dc-power-visa.svg'),
                    url: '#'
                },
            ]
        }
    }
}
</script>


<style lang=scss scoped>
@import '../styles/variables';

section {
    padding: 3rem 0;
    background-color: $brand_primary_color;

    ul {
        display: flex;
        justify-content: space-evenly;
        align-items: center;
    }

    img {
        vertical-align: middle;
        height: 3rem;
        max-width: 3.2rem;
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
