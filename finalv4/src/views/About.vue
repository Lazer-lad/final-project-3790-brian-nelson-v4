<template>
<v-container>
  <v-row>

<v-col cols='3' v-for="ship in starships" :key="ship.model">
<v-card>
  <v-card-title>
    <div>
      <h3>
        {{ ship.name }}
      </h3>
      <div> {{ ship.model }} </div>
      <p> {{ ship.manufacturer }} </p>
    
    </div>
  </v-card-title>
  <v-card-action>
    <v-btn @click="showing = false">hide</v-btn>
  </v-card-action>
</v-card>
</v-col>

  </v-row>
</v-container>
</template>

<script>
import { aboutMixin } from './aboutmixintest'

export default {
  data() { return 
    showing: false
  },
  mixins: [aboutMixin]
  
}
</script>