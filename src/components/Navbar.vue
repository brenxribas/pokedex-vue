<template>
  <v-container>
    <v-row>
      <v-container>
        <v-img
          :src="require('../assets/pokedex.png')"
          class="my-3"
          contain
          height="300"
        />
      </v-container>
    </v-row>

    <v-col class="mx-auto" cols="3">
      <v-text-field
        v-model="search"
        label="Pesquisar Pokémon"
        placeholder="Bulbasaur..."
        prepend-inner-icon="mdi-magnify"
        color="red"
        solo
      ></v-text-field>
    </v-col>
  </v-container>
</template>

<script>
export default {
  name: "Navbar",
  data() {
    return {
      search: ""
    }
  },
};
</script>