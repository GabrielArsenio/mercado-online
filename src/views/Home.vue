<template>
  <main class="home">
    <section
      id="banner"
      class="d-flex align-items-center flex-column justify-content-center"
    >
      <h1>Entrega em 2h!</h1>
      <span>Tenha sua comida na porta da sua casa</span>
      <div class="input-group mt-3">
        <input
          type="text"
          class="form-control"
          placeholder="Buscar por item ou marca"
          aria-label="Buscar por item ou marca"
          aria-describedby="button-addon2"
        />
        <button class="btn btn-primary" type="button" id="button-addon2">
          Buscar
        </button>
      </div>
    </section>
    <section id="categories">
      <Categories />
    </section>
  </main>
</template>

<script>
// @ is an alias to /src
import Categories from "@/components/Categories";

export default {
  name: "Home",
  components: {
    Categories,
  },
};
</script>

<style scoped>
#banner {
  height: 35vh;
  background-image: url("../assets/banner.png");
  background-size: cover;
  background-position: center;
}
</style>
