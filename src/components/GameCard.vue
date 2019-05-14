<template>
    <v-flex sm4 pa-4 align-space-between justify-space-around row fill-height>
        <v-card>
          <!-- <v-card-title primary-title>
            <h3 class="headline mb-0">{{game.title}}</h3>
          </v-card-title> -->
          <v-img style="max-height: 410px;"
            :src=game.image
          ></v-img>
          <v-card-text>
            {{game.description}}
          </v-card-text>
          <v-card-actions>
            <v-btn color="info">
              <v-icon>
                info
              </v-icon>
              Info
            </v-btn>
            <v-btn color="success">
              <v-icon>
                shopping_cart
              </v-icon>
              Kopen
            </v-btn>
            <v-spacer></v-spacer>
            <div class="text-xs-center">
              <v-chip color="red" text-color="white">&euro; {{game.price}}</v-chip>
            </div>
          </v-card-actions>
        </v-card>
      </v-flex>
</template>

<script>
export default {
    name: 'GameCard',
    props: {
      game: Object
    },
    data() {
      return {
        
      }
    },
    created() {
      
    }
}
</script>

<style>

</style>
