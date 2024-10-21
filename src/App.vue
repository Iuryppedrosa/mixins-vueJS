<template>
  <div style="display: flex; flex-direction: row">
    <div style="flex-basis: 33%">
      <ListaVideoGames />
    </div>

    <div style="flex-basis: 33%">
      <ListaFilmes />
    </div>

    <div style="flex-basis: 33%">
      <ListaPessoas />
    </div>
  </div>
</template>
<script>
import ListaVideoGames from './components/ListaVideoGames.vue'
import ListaFilmes from './components/ListaFilmes.vue'
import ListaPessoas from './components/ListaPessoas.vue'

export default {
  name: 'App',
  components: {
    ListaVideoGames,
    ListaFilmes,
    ListaPessoas,
  },
}
</script>

<style scoped></style>
