<script setup>
import fotografo from "../assets/fotografo.png";
</script>

<template>
    <section class="banner">
        <div>
             <h1>Onde a paisagem vira 
            <span>inspiração</span> .</h1>
            <p>Explore paisagens, cores e luzes que inspiram novas histórias através da fotografia.</p>
        </div>
       <img :src="fotografo" alt="Foto de uma fotografa">
    </section>
</template>

<style scoped lang="scss">
    .banner{
        //border: solid;
        display: flex;
        justify-content: space-between;
        margin: 2rem;


        h1{
            font-size: 3rem;

            span{
            color: #E1306C;
            font-size: 4.5rem;
        }
        }

        div{
            //background-color: aqua;
            width: 50%;
            display: flex;
            flex-direction: column;
            justify-content: center;
        }

    }
</style>