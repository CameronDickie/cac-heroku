<template>
  <!-- <v-card
    color="teal accent-1"
    flat
    height="200px"
    tile
  > -->
    <v-toolbar color="teal accent-1">
      <v-toolbar-title>Climate Action Carleton</v-toolbar-title>
      <v-spacer></v-spacer>
      <v-btn text large href="/home">Home</v-btn>
      <v-btn text large href="/about">About</v-btn>

      <!-- <v-btn icon>
        <v-icon>mdi-magnify</v-icon>
      </v-btn>

      <v-btn icon>
        <v-icon>mdi-heart</v-icon>
      </v-btn>

      <v-btn icon>
        <v-icon>mdi-dots-vertical</v-icon>
      </v-btn> -->
    </v-toolbar>
  <!-- </v-card> -->
</template>

<script>
  export default {
    name: 'Header',
    data () {
      return {}
    },
  }
</script>