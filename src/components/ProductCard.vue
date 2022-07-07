<template>
    <div class="col">
        <div class="product-card">
            <img :src="productDetails.thumb" :alt="productDetails.series">
            <h3 class="series">{{productDetails.series}}</h3>
        </div>
    </div>
</template>


<script>
export default {
    name: 'ProductCard',
    props: {
        productDetails: Object
    }
}
</script>


<style lang="scss" scoped>
@import '../styles/variables';

.col {
    width: calc(100% / 6);
    padding: 0 0.75rem;

    .product-card {
        cursor: pointer;
        margin-bottom: 3rem;
        text-align: center;

        img {
            object-fit: cover;
            object-position: top center;
            max-height: 10rem;
            margin-bottom: 1rem;
            width: 100%;
        }
        .series {
            color: white;
            font-size: 0.9rem;
            font-weight: 500;
            text-transform: uppercase;
            text-align: left;
        }
}
}

</style>









