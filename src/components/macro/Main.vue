<template>
    <main>
        <div class="container">
            <Products/>
        </div>
    </main>
</template>

<script>
import Products from '../sections/Products.vue';

export default {
    name: "Name",
    components: {
        Products,
    }
}
</script>

<style lang="scss" scoped>
    main {
        margin-top: 40px;
        background-image: url(../../assets/img/fondo-pag-speciali.jpg);
    }
</style>