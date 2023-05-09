<template>
    <div>
        <div id="header">
            <div class="container_items">
                <ul class="page_links">
                    <li>
                        <NuxtLink class="link" to="/products">Produtos</NuxtLink>
                    </li>
                    <li>
                        <NuxtLink class="link" to="/about">Sobre</NuxtLink>
                    </li>
                </ul>
                <div class="page_logo">
                    <h1>
                        <div>
                            <NuxtLink class="link title" to="/"> 
                                E-<span class="title_pt2">commerce</span>
                            </NuxtLink>
                        </div>
                    </h1>
                </div>
            </div>
        </div>
       <slot></slot>
    </div>
</template>

<script>
    export default{
        data(){
            return
        }
    }
</script>

<style scoped>
    .router-link-exact-active{
        color: #d11144;
    }
    #header{
        height: 60px;
        width: 100%;
        display: flex;
        align-items: center;
        justify-content: center;
        background-color: rgb(52, 174, 255);
        box-shadow: 0 0 15px rgba(0, 0, 0, 1);
    }
    .container_items{
        width: 95%;
        margin: 0 25px;
        display: flex;
        align-items: center;
        justify-content: space-between;
    }
    .page_links{
        list-style-type: none;
        gap: 35px;
        display: flex;
        justify-content: center;
    }
    .link{
        text-decoration: none;
        font-size: 24px;
        font-weight: bold;
        text-decoration: aliceblue;
        color: black;
    }
    .title{
        font-weight: bold;
        font-size: 30px;
        color: black;
    }
</style>