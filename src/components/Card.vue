<script setup>
defineProps(["imagem"]);
//o que é o defineProps
//é uma função do vue que permite receber dados em comunicação de componentes
import favoritos from "../assets/favoritos.png";
</script>

<template>
  <div class="card">
    <span class="fav"><img :src="favoritos" alt="" /></span>
    <img :src="imagem" alt="Imagem do card" />
  </div>
</template>

<style scoped lang="scss">
.card {
  //border: solid;
  position: relative;
  width: 15vw;
  height: 50vh;

  img {
    width: 100%;
    height: 100%;
    border-radius: 10px;
  }

  .fav {
    position: absolute;
    top: 8px;
    right: 8px;
    width: 15px;
    height: 15px;

    img {
      width: 100%;
      height: 100%;
    }
  }
}
</style>
