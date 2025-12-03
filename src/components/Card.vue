<script setup>
defineProps(["imagem"]);
//o que é o defineProps
//é uma função do vue que permite receber dados em comunicação de componentes
</script>

<template>

    <div class="card">
        <img :src="imagem" alt="Imagem do card">
    </div>
    
</template>

<style scoped lang="scss">
.card{
    //border: solid;
    width: 35vw;
   
    img{
        width: 100%;
        height: 100%;
        border-radius: 10px;
    }

    
}
</style>