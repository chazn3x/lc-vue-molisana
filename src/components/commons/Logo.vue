<template>
    <div class="logo">
        <img src="../../assets/img/la-molisana-logo.png" :alt="altText">
    </div>
</template>

<script>
export default {
    name: 'Logo',
    props: {
        altText: String,
    }
}
</script>

<style>

</style>