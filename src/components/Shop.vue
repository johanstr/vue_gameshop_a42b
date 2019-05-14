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
import { mapActions } from 'vuex'
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
    },
    methods: {

    }
  }
</script>

<style>

</style>
