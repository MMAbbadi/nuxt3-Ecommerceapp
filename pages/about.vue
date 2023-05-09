<template>
    <div class="body">
        <div class="container_infos">
            <div class="sobre">
            <h2>Sobre</h2>
            <p class="sobre_txt">
                Lorem ipsum dolor sit, amet consectetur adipisicing elit. Ipsum, magnam unde ducimus nam voluptate nisi expedita consequuntur iure hic. Illum libero culpa, expedita voluptates ut laboriosam excepturi! Harum, esse sit!
                Lorem ipsum dolor sit amet consectetur adipisicing elit. Esse, exercitationem inventore? Dignissimos aliquid iusto et nostrum labore quo repudiandae! Corporis ut blanditiis eum pariatur, id aspernatur aliquid quibusdam in deleniti!
                Lorem ipsum dolor sit amet consectetur adipisicing elit. Porro quia molestiae magni ipsam, quae deserunt ex molestias pariatur quis voluptatum eveniet velit error expedita voluptas. Dolorum incidunt nam deserunt eos.
                Lorem ipsum dolor sit amet consectetur adipisicing elit. Cupiditate ipsam quisquam cum fugiat illo! Aut minima impedit maiores ex eveniet maxime, necessitatibus repellendus modi nostrum! Harum pariatur suscipit quae iure!
            </p>
        </div>
        <div class="contatos">
            <h2>Contato</h2>
            <p>
                Lorem ipsum dolor sit amet, consectetur adipisicing elit. Exercitationem fuga modi temporibus animi ex delectus consequuntur maxime, ipsa, laudantium sint ea assumenda quam soluta perspiciatis atque earum vitae dolores. Error?
            </p>
            <p>
                Lorem, ipsum dolor sit amet consectetur adipisicing elit. Quod provident alias asperiores sequi porro quia, tenetur nobis quibusdam amet itaque quis earum nulla quo tempora non error accusamus voluptas eos.
            </p>
        </div>
        </div>
    </div>
</template>

<script setup>

</script>

<style scoped>
    .body{
        height: 909px;
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
        background: lightgreen;
    }
    .container_infos{
        width: 50%;
        height: 85%;
        padding: 10px;
        gap: 55px;
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
        background: rgba(255, 255, 255, 0.7);
        box-shadow: 0 0 15px rgba(0, 0, 0, 0.7);
    }
    h2{
        font-weight: bold;
        font-size: 40px;
    }
    p{
        text-justify: auto;
        font-size: 24px;
    }
    .sobre{
        gap: 15px;
        display: flex;
        flex-direction: column;
        align-items: center;
        justify-content: center;

    }
    .contatos{
        gap: 15px;
        display: flex;
        flex-direction: column;
        align-items: center;
        justify-content: center;
    }
</style>