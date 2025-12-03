<script setup>
import { Icon } from "@iconify/vue";
import logo from "../assets/logo.png";
import pessoa from "../assets/pessoa.png";
import pesquisa from "../assets/pesquisa.png"

</script>

<template>
<header>
    <img :src="logo" alt="Imagem da logo marca">
   <nav>
    <ul>
    <li>
        <a href="">
            <img :src="pesquisa" alt="Imagem de barra de pesquisa">
            <!-- <Icon class="search-icon" icon="material-symbols:search" /> -->
            <!-- <Icon icon="coleção:nomeDoIconeEmIngles" -->
        </a>
    </li>
    <li>
        <a href="">Início</a>
    </li>
    <li>
        <a href="">Galeria</a>
    </li>
    <li>
        <a href=""> Favoritos</a>
    </li>
    <li>
        <a href="">
            <img :src="pessoa" alt="">
        </a>
    </li>
    </ul>
   </nav>
</header>
</template>

<style scoped lang="scss">
header{
    //border: solid;
    display: flex;
    justify-content: space-between;
    align-items: center;
    flex-wrap: wrap;
    margin: 2rem;

    ul{
        display: flex;
        gap: 1.5rem;
       // border: solid;
        flex-wrap: wrap;
        list-style: none;
        align-items: center;
    }

    a{
        text-decoration: none;
        color: black;
    }
}


</style>