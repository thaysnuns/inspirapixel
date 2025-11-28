<script setup>
import { Icon } from "@iconify/vue";
import logo from "./assets/logo.png"

</script>

<template>
<header>
    <img :src="logo" alt="Imagem da logo marca">
   <nav>
    <li>
        <a href="">
            <Icon class="search-icon" icon="material-symbols:search" />
            <!-- <Icon icon="coleção:nomeDoIconeEmIngles" -->
        </a>
    </li>
    <li></li>
    <li></li>
    <li></li>
    <li></li>
   </nav>
</header>
</template>

<style scoped lang="scss">

</style>