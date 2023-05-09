<template>
    <div class="card">
        <img :src="product.image" alt="product thumb" class="thumb">
        <p class="product_title">
            {{ product.title.slice(0,15) }}
            <span v-if="product.title.length > 15">...</span>
        </p>
        <NuxtLink class="link" :to="`/products/${product.id}`">
            <p class="btn">Ver Produto</p>
        </NuxtLink>
    </div>
</template>

<script setup>
    const { product } = defineProps(['product'])
</script>

<style scoped>
    .card{
        min-height: 150px;
        padding: 15px;
        gap: 40px;
        display: flex;
        flex-direction: column;
        align-items: center;
        justify-content: center;
    }
    .thumb{
        min-height: 60px;
        max-width: 70px;
        margin: 0 auto;
    }
    .product_title, span{
        margin: 5px;
        font: bold;
        font-size: 20px;
        color: darkgray;
    }
    .link{
        text-decoration: none;
        font: bold;
        font-size: 20px;
    }
    .btn{
        display: flex;
        align-items: center;
        justify-content: center;
        width: 150px;
        color: white;
        padding: 3px 2px;
        border-radius: 10px;
        background: rgb(102, 205, 239);
    }
</style>