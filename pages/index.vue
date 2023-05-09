<template>
    <div class="container">
        <div class="bg_pagina">
            <div class="container_conteudo_pagina">
                <div class="container_titulo_site">
                    <h1 class="titulo_site">Some Text</h1>
                    <h3 class="sutitulo_site">Mais texto aqui</h3>
                </div>
                <NuxtLink class="btn_produtos" to="/products">
                    <div >ver produtos</div>
                </NuxtLink>
            </div>
        </div>

    </div>
</template>

<script setup>

</script>

<style>
    *{
        margin: 0;
        padding: 0;
        box-sizing: border-box;
        font-family: Arial, Helvetica, sans-serif;
    }
    .container{
        height: 909px;
        display: flex;
        align-items: center;
        flex-direction: column;
        justify-content: center;
    }
    .bg_pagina{
        width: 100%;
        height: 100%;
        display: flex;
        align-items: center;
        flex-direction: column;
        justify-content: center;
        background-color: rgb(32, 32, 110);
        background-image: url('~/assets/imagens/bg.jpg');
        background-position: center;
        background-size: cover;
        z-index: 0;
    }
    .container_conteudo_pagina{
        width: 25%;
        height: 75%;
        gap: 10%;
        position: relative;
        right: -30%;
        display: flex;
        align-items: center;
        flex-direction: column;
        justify-content: center;
        background: rgba(255, 255, 255, 0.7);
        box-shadow: 0 0 15px rgba(0, 0, 0, 0.7);
    }
    .container_titulo_site{
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;

    }
    .titulo_site{
        font-size: 45px;
    }
    .btn_produtos{
        width: 150px;
        height: 40px;
        display: flex;
        align-items: center;
        justify-content: center;
        border-radius: 25px;
        border: solid 1px rgb(169, 169, 169);
        background: rgb(97, 220, 97);
        text-transform: uppercase;
        font-weight: bold;  
        cursor: pointer;
        text-decoration: none;
        color: rgb(98, 98, 98);
    }
</style>