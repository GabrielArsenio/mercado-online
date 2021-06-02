<template>
  <ul>
    <li v-for="category of categories" :key="category.id">
      <img
        :src="category.img"
        class="rounded-circle"
        height="80"
        alt="Category"
      />
      <div class="name-container">
        <span>{{ category.name }}</span>
      </div>
    </li>
  </ul>
</template>

<script>
export default {
  name: "Categories",
  data() {
    return {
      categories: [
        {
          id: 1,
          img:
            "https://static-images.ifood.com.br/image/upload//mercados/categorias/carne.png",
          name: "Carnes, Aves e Peixes",
        },
        {
          id: 1,
          img:
            "https://static-images.ifood.com.br/image/upload//mercados/categorias/basicos.png",
          name: "Alimentos Básicos",
        },
        {
          id: 1,
          img:
            "https://static-images.ifood.com.br/image/upload//mercados/categorias/bebidas.png",
          name: "Bebidas",
        },
        {
          id: 1,
          img:
            "https://static-images.ifood.com.br/image/upload//mercados/categorias/bebidas_alcool.png",
          name: "Bebidas Alcoólicas",
        },
        {
          id: 1,
          img:
            "https://static-images.ifood.com.br/image/upload//mercados/categorias/congelados.png",
          name: "Congelados",
        },
        {
          id: 1,
          img:
            "https://static-images.ifood.com.br/image/upload//mercados/categorias/feira.png",
          name: "Feira",
        },
        {
          id: 1,
          img:
            "https://static-images.ifood.com.br/image/upload//mercados/categorias/frios.png",
          name: "Frios e Laticínios",
        },
        {
          id: 1,
          img:
            "https://static-images.ifood.com.br/image/upload//mercados/categorias/leite.png",
          name: "Leites e Iogurtes",
        },
        {
          id: 1,
          img:
            "https://static-images.ifood.com.br/image/upload//mercados/categorias/matinais.png",
          name: "Matinais",
        },
        {
          id: 1,
          img:
            "https://static-images.ifood.com.br/image/upload//mercados/categorias/padaria.png",
          name: "Padaria",
        },
        {
          id: 1,
          img:
            "https://static-images.ifood.com.br/image/upload//mercados/categorias/biscoitos.png",
          name: "Biscoitos e Salgadinhos",
        },
        {
          id: 1,
          img:
            "https://static-images.ifood.com.br/image/upload//mercados/categorias/doces.png",
          name: "Doces e Sobremesas",
        },
        {
          id: 1,
          img:
            "https://static-images.ifood.com.br/image/upload//mercados/categorias/limpeza.png",
          name: "Limpeza",
        },
        {
          id: 1,
          img:
            "https://static-images.ifood.com.br/image/upload//mercados/categorias/higiene.png",
          name: "Higiene e Cuidados Pessoais",
        },
      ],
    };
  },
};
</script>

<style scoped>
ul {
  list-style-type: none;
  display: flex;
  overflow-y: auto;
  padding: 20px;
}

li {
  padding: 0 10px;
  display: flex;
  flex-direction: column;
  align-items: center;
}

.name-container {
  text-align: center;
  font-size: 0.75em;
}
</style>