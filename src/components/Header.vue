<template>
    <v-toolbar color="primary">
      <v-img src="../assets/logo-content/noir-sapling.png" max-height="80px" max-width="70px"></v-img>
      <v-toolbar-title>Climate Action Carleton</v-toolbar-title>
      <v-spacer></v-spacer>
      <v-btn text large href="/home">Home</v-btn>
      <v-btn text large href="/about">About</v-btn>
    </v-toolbar>
</template>

<script>
  export default {
    name: 'Header',
    data () {
      return {}
    },
  }
</script>