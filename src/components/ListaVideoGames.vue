<template>
  <div>
    <h3>Lista Video Games</h3>
    <input
      type="test"
      placeholder="Digite o nome do video game"
      v-model="item"
      @keyup.enter="adicionarItem"
    />
    <ul>
      <li v-for="item in itens" :key="item">
        {{ item }}
        <button @click="removerItem(item)">X</button>
      </li>
    </ul>
  </div>
</template>
<script>
import listaMixin from '@/mixins/listaMixin'
import removerItemLista from '@/mixins/removerItemLista'
export default {
  name: 'ListaVideoGames',
  mixins: [listaMixin, removerItemLista],
}
</script>
