<template>
    <div class="card">
        <div class="container_pagina">
            <div class="container_conteudo">
                <div class="imagem_container">
                    <img :src="product.image" alt="product img" class="item_img">
                </div>
            </div>
            <div class="container_infos">
                <h2 class="title_item">{{ product.title }}</h2>
                <h3 class="item_price">Preço: R${{ product.price }}</h3>
                <h3 class="item_description">Sobre o produto:</h3>
                <p class="descirption_body">{{ product.description }}</p>
            </div>
        </div>
    </div>
</template>

<script setup>
    const { product } = defineProps(['product'])
</script>

<style scoped>
.card{
    height: 909px;
    gap: 250px;
    display: flex;
    align-items: center;
    justify-content: center;
}
.container_pagina{
    height: 870px;
    width: 97%;
    display: flex;
    align-items: center;
    justify-content: center;
    box-shadow: 0 0 80px rgba(0, 0, 0, 0.8);
}
.container_conteudo{
    height: 100%;
    width: 50%;
    padding: 15px;
    display: flex;
    align-items: center;
}
.imagem_container{
    height: 100%;
    width: 650px;
    display: flex;
    align-items: center;
    justify-content: center;
    padding: 5px 5px;
    margin: 30px 30px;
}
.item_img{
    height: 100%;
    width: 100%;
}
span{
    font-weight: bold;
}
.container_infos{
    height: 80%;
    width: 50%;
    padding: 10px;
    margin: 30px 20px;
    display: flex;
    flex-direction: column;
    gap: 15px;
}
.title_item{
    height: 120px;
    font-size: 40px;
}
.item_price{
    height: 60px;
    font-weight: 500;
    font-size: 30px;
}
.item_description{
    height: 30px;
    border-bottom: 2px solid rgb(232, 232, 232);  

}
.descirption_body{
    height: 30%;
}
</style>