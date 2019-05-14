<template>
  <v-container>
    <v-layout wrap>
      <GameCard v-for="game in games" 
        :key="game.id" 
        :game="game" />
    </v-layout>
  </v-container>
</template>

<script>
import GameCard from './GameCard'

  export default {
    name: 'Shop',
    props: {
      games: Array
    },
    components: {
      GameCard
    },
    data() { 
      return {
        
      }
    }
  }
</script>

<style>

</style>
