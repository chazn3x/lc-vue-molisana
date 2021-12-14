<template>
    <div class="product">
        <img :src="product.src" :alt="product.titolo + ' immagine'">
        <h3>{{product.titolo}}</h3>
        
    </div>
</template>

<script>
export default {
    name: "CardProduct",
    props: {
        product: Object,
    }
}
</script>

<style lang="scss" scoped>
    .product {
        background-color: #fff;
        padding: 20px 15px;
        h3 {
            text-align: center;
        }
        img {
            width: 100%;
        }
    }
</style>