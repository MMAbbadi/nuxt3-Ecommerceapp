<template>
    <div>
        <div class="container_produtos">
            <div v-for=" p in products" class="produtos">
                <ProductCard :product="p" />
            </div>
        </div>
    </div>
</template>

<script setup>
//fetch products
    const { data:products } = await useFetch('https://fakestoreapi.com/products')
</script>

<style scoped>
    .container_produtos{
        height: 909px;
        padding: 30px 0 10px 35px;
        display: grid;
        row-gap: 30px;
        grid-template-columns: 1fr 1fr 1fr 1fr;
        align-items: center;
        justify-content: center; 
    }
    .produtos{
        width: 85%;
        padding: 15px;
        border-radius: 5px;

        box-shadow: 0 0 5px rgba(0, 0, 0, 0.6);
    }
</style>