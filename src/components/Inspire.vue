<script setup>
import Card from "./Card.vue";
//importamos o axios -> biblioteca para fazer requisições HTTP
import axios from "axios";

//importamos o ref -> uma ferramenta que permite criar variaveis reativas
import { ref } from "vue";

//criar uma variave reativa que vai receber a lista de imagens da API
const imagens = ref([]);

//função assincrona -> pra buscar a API
async function carregarImagens() {
  //res -> resposta da API
  //axios pega os dados get axios.get()
  //await vc precisa esperar o axios ir buscar as imagens
  const res = await axios.get("https://picsum.photos/v2/list?page=5&limit=30");

  imagens.value = res.data;
  //guardando as imagens da API dentro da variavel imagens
  //
  console.log(res);
}

carregarImagens();
</script>

<template>
  <h2>Inspire-se</h2>
  <section class="inspire">
    <Card v-for="img in imagens" :imagem="img.download_url" />
  </section>
</template>

<style scoped lang="scss">
h2 {
  //justify-content: space-evenly;
  margin: 2rem;
}

.inspire {
  display: flex;
  gap: 10px;
  flex-wrap: wrap;
  justify-content: space-around;
  margin: 2rem;
}
</style>
