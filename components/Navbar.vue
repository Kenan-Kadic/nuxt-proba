<template>
  <div class="Navbar">
    <v-app-bar text app>
      <v-app-bar-nav-icon class="red--text" @click="drawer = !drawer"></v-app-bar-nav-icon>
    <v-app-bar-title class="text-uppercase grey-- text text-no-wrap">
      <span class="font-weight-light">Todo</span>
        <span>Ken</span>
    </v-app-bar-title>
        <v-spacer></v-spacer>
      <v-btn text color="grey lighten-3">
      <span>Sign Out</span>
      <v-icon right>mdi-arrow-right-bold-box-outline</v-icon>
      </v-btn>
      </v-app-bar>

      <v-navigation-drawer app v-model="drawer" class="red">
        <p>test</p>
      </v-navigation-drawer>
  </div>
</template>

<script>
  export default {
    data() {
      return {
        drawer: false
      }
    }
  }
</script>
