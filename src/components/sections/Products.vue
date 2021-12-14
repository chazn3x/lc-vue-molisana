<template>
    <section>
        <h2>Lista Prodotti</h2>
        <div class="products-list">
            <CardProduct v-for="(product, index) in products" :key="index" :product="product"/>
        </div>
    </section>
</template>

<script>
import CardProduct from '../commons/CardProduct.vue';
import Products from '../../data/products.js';
export default {
    name: "Products",
    components: {
        CardProduct,
    },
    data() {
        return {
            products: Products,
        }
    }
}
</script>

<style lang="scss" scoped>
    section {
        h2 {
            text-align: center;
            margin: 20px 0;
        }
        .products-list {
            display: flex;
            flex-wrap: wrap;
        }
    }
</style>