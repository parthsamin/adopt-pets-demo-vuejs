<template>
    <div id="app">
        <h1> Cats for Adoption </h1>
        <v-app id="inspire">
        <v-data-table
            :headers="headers"
            :items="cats"
        ></v-data-table>
  </v-app>
    </div>
</template>

<script>
import cats from '@/data/cats'

export default {
  data () {
    return {
      headers: [
        { text: 'Name', value: 'name' },
        { text: 'Breed', value: 'breed' },
        { text: 'Species', value: 'species' },
        { text: 'Gender', value: 'gender' },
        { text: 'Age', value: 'age' },
        { text: 'Color', value: 'color' },
        { text: 'Weight', value: 'weight' },
        { text: 'Location', value: 'location' },
        { text: 'Notes', value: 'notes' }
      ],
      cats
    }
  }

}
</script>
