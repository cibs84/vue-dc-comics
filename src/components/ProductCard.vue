<template>
    <div class="product-card">
        <img :src="productDetails.thumb" :alt="productDetails.series">
        <h3 class="series">{{productDetails.series}}</h3>
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

.product-card {
    width: calc((100% / 6) - 1.5rem);
    margin-bottom: 3rem;
    cursor: pointer;

    img {
        object-fit: cover;
        object-position: top center;
        width: 100%;
        height: 11.3rem;
        margin-bottom: 1rem;
    }
    .series {
        color: white;
        font-size: 0.9rem;
        font-weight: 500;
        text-transform: uppercase;
    }
}

</style>









