

<template>
<v-container>
  <v-row>

<v-col cols='3' v-for="ship in starships" :key="ship.model">
<v-card>
  <v-card-title>
    
      
        <p class="text-no-wrap">{{ ship.name }}</p>
      
        </v-card-title>

      <v-card-subtitle>
        <div> {{ ship.model }} </div>
      </v-card-subtitle>
      <v-card-text> {{ ship.manufacturer }} </v-card-text>
    
    
  
  <v-card-action>
    <v-btn class='mx2' fab dark small color="primary" @click="showing = false"><v-icon dark>mdi-minus</v-icon></v-btn>
  </v-card-action>
</v-card>
</v-col>

  </v-row>
</v-container>
</template>

<script>
import { aboutMixin } from './aboutmixintest'

export default {
  data() { 
    return {
    showing: false
    }
  },
  mixins: [aboutMixin]
  
}
</script>