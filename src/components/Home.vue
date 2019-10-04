<template>
  <div>
    <h1 class="display-3 font-weight-light mb-4">Negocios e Consultas de Ações</h1>
    <v-sheet :elevation="6" class="pa-2 primary blue darken-1" color="primary">
      <v-icon class="white--text mr-3">info</v-icon>
      <span>Você pode salvar e carregar os dados</span>
    </v-sheet>
     <v-sheet :elevation="6" class="pa-2 primary success darken-1" color="primary">
      <v-icon class="white--text mr-3">info</v-icon>
      <span>Você pode salvar e carregar os dados</span>
    </v-sheet>
    <v-divider class="my-4" />
    <p><strong>Seu Saldo:</strong> {{ funds | currency }}</p>
  </div>
</template>

<script>
export default {
  computed: {
    funds(){
      return this.$store.getters.funds
    }
  }
}
</script>

<style>

</style>