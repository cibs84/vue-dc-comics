<template>
    <section class="products-section">
        <div class="container">
            <!-- Category Label -->
            <h2 class="category-label"> Current Series</h2>

            <!-- All Products -->
            <div class="products-list">
                <ProductCard v-for="product, index in productsArray" :key="index" :productDetails="product"/>
            </div>

            <!-- Load More Button -->
            <button class="load-more">Load More</button>
        </div>
    </section>
</template>


<script>
import ProductCard from './ProductCard.vue';
import productsJson from '../assets/dc-comics.json'

export default {
    name: 'ProductsSection',
    components: {
        ProductCard
    },
    data() {
        return {
            productsArray: productsJson
        }
    }
}
</script>


<style lang="scss" scoped>
@import '../styles/variables';

section {
    padding: 3rem 0 1.2rem;
    background-color: $almost_black;

    .container {
        position: relative;

        .category-label {
            position: absolute;
            top: -4.7rem;
            left: -1rem;
            padding: 0.6rem 2rem;
            text-transform: uppercase;
            color: #fff;
            font-weight: 700;
            font-size: 1.7rem;
            background-color: $brand_primary_color;
        }
        .products-list {
            display: flex;
            flex-wrap: wrap;
            justify-content: space-between;
        }
        button {
            background-color: $brand_primary_color;
            border: none;
            color: #fff;
            text-transform: uppercase;
            padding: 0.7rem 3rem;
            font-size: 0.8rem;
            font-weight: 700;
            cursor: pointer;
            margin: 0 auto;
            display: block;
        }
    }
}

</style>









