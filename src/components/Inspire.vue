<script setup>
import Card from "./Card.vue";
</script>

<template>
  <h2>Inspire-se</h2>
  <section class="inspire">
    <Card
      imagem="https://i.pinimg.com/736x/cc/0d/37/cc0d3781240d0fbfe57194dd56898c88.jpg"
    />
    <Card
      imagem="https://i.pinimg.com/236x/2a/bd/f1/2abdf10d67683fc2354f5aeac3b9a69c.jpg"
    />
    <Card
      imagem="https://www.publicdomainpictures.net/pictures/280000/nahled/night-landscape-1546338197B2k.jpg"
    />
  </section>
</template>

<style scoped lang="scss">
.inspire, h2{
    display: flex;
    justify-content: space-between;
    gap: 10px;
    margin: 2rem;
}
</style>